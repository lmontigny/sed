```
Character 	Description
^ 	Matches the beginning of the line
$ 	Matches the end of the line
. 	Matches any single character
* 	Will match zero or more occurrences of the previous character
[ ] 	Matches all the characters inside the [ ] 
```
```
[a-z]       = [[:lower:]]
[A-Z]       = [[:upper:]]
[a-zA-Z]    = [[:alpha:]]
[0-9]       = [[:digit:]]
[a-zA-Z0-9] = [[:alnum:]]
```

# Example

- Delete all spaces at the end of every line.  
`sed 's/ *$//' input`

- Zero or more numbers (so the first char as it matches 0 numbers)  
`sed 's/[0-9]*/(&)/' song.txt`

- A number (with extended regular expression)  
`sed -r 's/[0-9]+/(&)/' song.txt`

