# API Routes

## GET
### /[GPSCoordinates]/nearby
Uses the user's approximate location (heavily rounded for anonymity) and returns a JSON list of all posts within a standard radius of the coordinates.

### /recent 
Returns a list of X number of most recently approved images.

### /[User]/gallery
Returns a JSON object that contains a list of the user's posts.

### /[User]/home
Returns a JSON object containing both recently approved images and nearby.

### /voting
Returns a the JSON representing a random image in our system currently being voted on. Has a POST counterpart to recieve that data.

### /voting/[image ID]
Same as `/voting` except it directly links to the voting of a particular image.


## POST
All POST submissions are verified by login.

### /submit
Recieves the image upload from the user.

### /voting
Recieves a user's votes and suggestions on an image.

### /settings
Allows the user to update an user-specific settings.


