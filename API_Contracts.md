# MOBITE API Contracts

### Default Headers for each request
```
  "X-Api-Request": true,
  "Accept: "application/json"
```

If user is authorized, add 
```
  "Authorization": "Bearer jwt_token"
```
Where instead of `jwt_token`, an actual token is provided.

---

If `X-Api-Request` header is not provided, API should redirect to landing page.

If response code is **not** `200`, error object is returned:

```json
  {
    "type": 404,
    "title": "string",
    "details": "string"
  }
```

---

**`GET /api/v1/questions/{id}`**

Code 200
```json
  {
    "title": "string",
    "answers": [
      {
        "answer": "string",
        "img_url": "string",
        "next_question_id": 0
      }
    ],
  }
```

---

**`GET /api/v1/recommendation`**

[TBA]

---

**`POST /api/v1/signup`**

Body
```json
{
  "email": "string",
  "username": "string",
  "password": "string"
}
```

Code 200
```json
{
  "token": "string"
}
```

---

**`POST /api/v1/users/login`**

Body
```json
{
  "email": "string",
  "username": "string",
  "password": "string"
}
```

Code 200
```json
{
  "token": "string"
}
```

---

**`GET /api/v1/quiz`**

Code 200
```json
  {
    "data":
    {
      "message": "string" 
    }
  }
```
