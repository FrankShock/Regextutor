# Regex Email Matching Tutorial

In my  Tutorial I will be going over the common Regular expression and describe the Matching Email Regular Expression. 

## Summary

A regular expression is a sequence of characters that defines a search pattern. This is commonly used to find patterns within a string, find/replace characters within a string or validate input.
The expression looks like this: `/^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/`


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors
The anchors we use in this regex expression for matching an email are `^ `, which starts the string and `$`to indicate the ending of the string.
Because our regular expression contains both, a given string must match all the given specifications exactly, or it won't be a match.

### Quantifiers
The Quantifiers are used to determine how many times a given character is suppose to appear.
In this  regex we use the `+` operator, which will connect the users email name + email service + `.com`. We also use for this regex includes `{2,6}`, which will allow you match range of 2-6 characters for the character set of `[a-z\.]`.

### Character Classes
In Regex expressions they use special character classes that match types of characters. class in this expression is `\d`, which matches a single characters that is a digit from 0-9. Though we have  one character class in the expression, the form-changing function of a backslash is useful in understanding another frequently used part of the expression, ".".

### Grouping and Capturing
In Regex expressions they use () for Grouping and capturing. 
The information/characters in the set of parentheses is taken as a single group, which allows all the information inside to be treated as a single entity. In a way you could view this expression of having 3 different groups. 
### Bracket Expressions
I  this expression we use/have three bracket expressions. these are [a-z0-9_.-], [\da-z.-], and [a-z.]. The character within the brackets can be anything specified. So, to use for example, in [a-z0-9_.-], this character will be matched by any lowercase letters from a-z, any digit from 0-9, or a period.

## Author
You can view my projects at https://github.com/FrankShock
