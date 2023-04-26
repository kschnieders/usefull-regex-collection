## To validate a Discord username
+ The name may be between 2 and 28 characters long.
+ The name may only consist of letters, numbers, underscores and spaces.
+ Spaces can optionally be present at the beginning of the name.
+ An ID with the # sign and four numbers must be present at the end of the name.
```
^\s*[a-zA-Z0-9_ ]{2,28}#[0-9]{4}$
```
## To validate a Twitch username
+ The string consists of 4 to 25 characters.
+ The string contains only letters (upper and lower case), numbers and underscores.
+ The string is case sensitive.
```
^[a-zA-Z0-9_]{4,25}$
```
