# Week Report 6

## Summary of Presentation : 

- **Wildcards**
A wildcard is a character that can be used in a search to replace any of a group of characters, considerably boosting the flexibility and efficiency of searches.

|Wilcard | meaning                                                                                                                          | Example             |
|--------|----------------------------------------------------------------------------------------------------------------------------------|---------------------|
|*       |It matches anything and nothing matches any number of characters                                                                  | ls *.txt            |
|?       |In shell commands, is used as a wildcard character to indicate exactly one character or more, which can be any single character.  |   ls t?.txt         |
|[]      |It matches a single character in a range                                                                                          | ls p[aeiou]*        |
|[!]     |It matches all except what is inside the brackets                                                                                 | ls [ae]*            |
![cheatsheetwildcard](../../cheat%20sheets/WILDCARDS_FILE%20GLOBBING%20CHEAT%20SHEET.png)

- **Brace expansion and how to use it**
This is a feature of bash that allows to generate arbitrary string to use with commands.

Example, `mkdir -p music/{jazz,rock}/{m3files,videos}new{1..3}`
Example removing multiple files: `rm -r {text1.tx,text2.txt,text3.txt}`

