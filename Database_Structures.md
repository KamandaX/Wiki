PHONE|
-|
id|
manufacturer|
model_name|
display_resoliution|
price|
launch_date|
screen_size|
protection_rating|
processor|
storage|
ram|
battery_size|

CAMERA|
-|
fk_phoneid|
side {main, selfie}|
megapixels|
f-number|

SCORES|
-|
fk_phoneid|
processing_power_scr|
main_camera_scr|
selfie_camera_scr|
storage_scr|
battery_life_scr|
durability_scr|
popularity_scr|
screen_size|
price|

QUESTION|
-|
id|
question_content|
aspect {processing_power, main_camera, selfie_camera, storage, battery_life, durability, popularity, screen_size, price}|

QUESTION_OPTION|
-|
fk_questionid|
option_content|
picture_link|
qustion_multiplier|

USER|
-|
id|
email|
username|
registered_at|
