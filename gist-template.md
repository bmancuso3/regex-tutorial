# Regex Tutorial - Matching an Email

Ever wondered what that strange character grouping called a regular expression is or what it does?  In this tutorial, we will look at the meaning behind the characters that comprise the regex for matching an email.

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
- [Conclusion](#conclusion)

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
Grouping constructs are also not used in this specific match an email regex, but they are commonly found in regexes as a whole.  Parentheses ```( )``` are the main syntax for grouping and are used to group strings in what is called a subexpression. 

The purpose of subexpressions is to search for the specific string that is contained within the parentheses.

### Bracket Expressions
Bracket expressions are the most important component of this match an email regex and are introduced with square brackets ```[ ]```.  The contents of the square brackets indicate a range of characters that the expression is searching for, in this case:

```[a-zA-Z0-9+_.-]``` and ```[a-zA-Z0-9.-]```.

Bracket expressions are rather straighforward when compared with other components of a regex, as the character ranges are specified within the expression.  

This first part of the regex is looking for any character ```a``` to ```z```, capital or lower case, any number ```0``` to ```9```, and it also accepts ```+```, ```_``` , ```.```, and ```-```.

The second part of the regex is similar to the first and is looking for any character ```a``` to ```z```, capital or lower case, any number ```0``` to ```9```, and it also accepts ```.```, and ```-```.  This section, following the ```@```, represents the "organization.com" portion of the email address, which is why it accepts fewer characters than the first section.

### Character Classes
Character classes are a more technical way of introducing a set of characters and fulfill essentially the same puprose as bracket expressions, but with greater efficiency.  They are not used in this regex, however.

### The OR Operator
There are no OR operators in this regex.  The OR operator, ```|```, is used to add flexibility into grouping constructs and bracket expressions.

### Flags
Flags are placed at the end of a regex outside of the ```\```.  They impose additional limits and functionality, but are not included in this match an email regex.

### Character Escapes
A character escape, identified by a ```\``` within the expression, is used to tell the regex to ignore the special properties of a character and to look for that character.  There are no character escapes in this regex, though!

### Conclusion
One additional facet of this regex are the two ```+``` signs.  They signify that the preceding bracket expressions can be repeated, therefore there can be multiple instances of any character within the range specified. 

The final note for this regex is that the ```@``` is reflected as itself within the expression.  If you have an email address, you can visualize this!

We have gone over each portion of this match an email regex:
```
/^[a-zA-Z0-9+_.-]+@[a-zA-Z0-9.-]+$/
```
It is a fairly straightforward expression, so for deeper learning, you'll have to hit the web.  Good luck!

## Author

Robert Mancuso is a Full Stack Web Developer with a background as an Infantry Officer in the US Army and West Point graduate. Eager to continue learning and developing, both personally and professionally, Robert has embarked on a new career path in the world of coding.

### <a href="https://github.com/bmancuso3/regex-tutorial">GitHub Repository</a>
