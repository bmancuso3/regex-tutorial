# Regex Tutorial - Matching an Email

Ever wondered what that strange character grouping called a regular expression was?  In this tutorial, we will look at the meaning behind the characters that comprise the regex that matches an email.

## Summary

The match an email regex is most commonly used to verify an email address, character for character.  We will explore what each portion of this regex means as it pertains to the email address being validated.  For starters, here is the match an email regex:
```
/^[a-zA-Z0-9+_.-]+@[a-zA-Z0-9.-]+$/
```

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
Anchors, also called assertions, are used to signify the beginning and end of the expression.  They are used to add structure and precision to the expression by limiting the acceptable threshold of matching.  
The anchors in the matching an email regex are ```^``` and ```$```.
The ```^``` signifies the beginning of the string, where all the characters that follow it must fit within the upcoming parameters (which we will get to).
The ```$``` signifies the end of the string, where all the characters that precede it must fit within the parameters declared.
Effectively, the anchors comprise the bookends of the string, ensuring the parameters within the email match the criteria exactly. 

### Quantifiers
This match an email regex does not use any quantifiers, but they are generally used to impose limits on the string as a whole.
Some quantifier examples are ```*, +, ?,``` and ```{ }```, with each one behaving in its respective manner, which you'll have to google.

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

Robert Mancuso is a Full Stack Web Developer with a background as a West Point graduate and Infantry Officer in the US Army. Eager to continue learning and developing, both personally and professionally, Robert has embarked on a new career path in the world of coding.

### <a href="https://github.com/bmancuso3/regex-tutorial">GitHub Repository</a>
