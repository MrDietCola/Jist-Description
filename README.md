# AJ Seidler /^[\+]?[(]?[0-9]{3}[)]?[-\s\.]?[0-9]{3}[-\s\.]?[0-9]{4,6}$/im

/^[\+]?[(]?[0-9]{3}[)]?[-\s\.]?[0-9]{3}[-\s\.]?[0-9]{4,6}$/im   
This is a regex for finding a phone number in a string. 

## Summary

The regex I will be walking you through today will be finding a phone number in a body of text. This regex will be able to find a phone number even if it is in a handful of different formats. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
The '^' indicates to anchor the regex to the start of a line of text. The '$' anchor indicates the end of the input line. These anchors will ensure that the search does not carry from one line into another. 

### Quantifiers
This regex uses quantifiers in three different spots to get the numbers that match a telephone number sequence of 3, 3, and 4. In the regex, we can se the use of [0-9], followed by {3}, this is telling us that we are looking for any characters between 0 and 9, where it is repeated three times in a row. We can also see the same search characters but followed by {4,6}. This is telling us to look for any characters between 0-9 that are repeating 4 to 6 times in a row. 

### Grouping Constructs
This regex does not include any grouping constructs

### Character Classes
This regex is using a few different character classes.  

* [\+] This is looking for a '+' character  
* [(] This is looking for '('  
* [0-9] This is looking for any number between 0-9  
* [)] This is looking for ')'   
* [-\s\.] This is looking for a '-' or ' ' or '.' character  

### The OR Operator
This regex does not use the OR operator 

### Flags
This regex uses 'i' to indicate that the regex is case sensitive and will look for both uppercase and lowercase letters seperately. The 'm' in the expression uses multi-line mode, which makes the regex search across each line. 

### Character Escapes
The character escapes included in this regex are '\+' and '\.'. The character escapes here are looking for a literal plus sign or a literal period. 

## Author
I have been able to use this to find various telephone numbers in a body of text. 

Here is a link to my GitHub. 
https://github.com/MrDietCola