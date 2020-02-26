## Coding Style
* Use https://www.dofactory.com/reference/csharp-coding-standards as a reference. Setup your IDE to apply these rules.
* Use 4 spaces instead of a tab.
* Brackets can be ommited if the body consists of one line.
    ```
    // Correct
    if (clause)
    {
        // Statements
    }
    // Also correct
    if (clause)
        // Statement
    // Avoid
    if (clause) { /* Statement */ }
    ```
* Access modifiers should be typed explicitly.
    ```
    // Correct
    internal class Example
    {
        private int _number;
    }
    // Avoid
    class Example
    {
        int _number;
    }
    ```
* Private variables should be named with `_camelCase`.
    ```
    // Correct
    private int _number;
    // Avoid
    private int number;
    private int Number;
    ```
* Static variables and constants should be named with `PascalCase`.
    ```
    // Correct
    public static string ApiUrl;
    public const int Year = 2020;
    // Avoid
    public static string apiUrl;
    public const int year = 2020;
    ```
* Classes should have `internal` access modifier unless it must absolutely be exposed. 
* Public fields and methods should have `public` access modifier.
## Testing
[TBD]
## Error reporting
* Use [Sentry](https://sentry.io/for/csharp/) for error reporting.
## IDE 
* [Microsoft Visual Studio 2019](https://visualstudio.microsoft.com/vs/) is highly recommended.
* [Resharper extension](https://www.jetbrains.com/resharper/) is highly recommended.
