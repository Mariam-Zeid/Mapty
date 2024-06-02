# Notes

- "this" context is lost when the \_loadMap function is called as a callback. 

- In JavaScript, "this" inside a callback function does not refer to the instance of the class unless it is explicitly bound.

- _loadMap method is passed as a callback to navigator.geolocation.getCurrentPosition. To ensure this refers to the App instance inside _loadMap, you need to bind this when passing _loadMap as a callback

- Event Listeners Inside Constructor 