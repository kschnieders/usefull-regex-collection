## To validate a Discord username
+ The name may be between 2 and 28 characters long.
+ The name may only consist of letters, numbers, underscores, spaces, pipe symbol and "()".
+ Spaces can optionally be present at the beginning of the name.
+ An ID with the # sign and four numbers must be present at the end of the name.
```
^\s*[a-zA-Z0-9_() |]{2,28}#[0-9]{4}$
```
## To validate a Twitch username
+ The string consists of 4 to 25 characters.
+ The string contains only letters (upper and lower case), numbers and underscores.
+ The string is case sensitive.
```
^[a-zA-Z0-9_]{4,25}$
```
## To validate a YouTube url
+ Checks whether a string contains a valid YouTube URL.
+ Starts at the beginning of the string.
+ Optionally checks if the URL starts with "http://" or "https://".
+ Optionally checks if "www." occurs in the URL.
+ Searches for "youtube.com/watch?v=" or "youtube.com/embed/" or "youtu.be/" in the string.
+ If one of these cases is true, the regex expects the YouTube video ID code.
+ The YouTube video ID code must contain exactly 11 letters, numbers, underscores, or hyphens.
+ Once all these conditions are met, the URL is recognized as valid.
```
^(?:https?:\/\/)?(?:www\.)?(?:youtube\.com\/(?:watch\?v=|embed\/)|youtu\.be\/)([a-zA-Z0-9_-]{11})$
```
