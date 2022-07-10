# Regex Tutorial

Regular expressions are a way to describe patterns in a string data. Regular expressions allow programmers to check a string of characters for patterns, to verify so if the pattern matches the criteria defined by that regular expression and produce actionable information.

## Summary

We will be covering RegExp.prototype.exec().
This method returns an array containing all the matched groups. It accepts a string that the programmer must test against a regular expression.

var regex = /^(\d{1,2}-){2}\d{2}(\d{2})?$/;
console.log(regex.test('01-01-1990'));
// true
console.log(regex.test('01-01-90'));
// true
console.log(regex.test('01-01-190'));
// false


## Table of Contents

- [Regex Tutorial](#regex-tutorial)
  - [Summary](#summary)
  - [Table of Contents](#table-of-contents)
  - [Regex Components](#regex-components)
    - [Anchors](#anchors)
    - [Grouping and Capturing](#grouping-and-capturing)
    - [Bracket Expressions](#bracket-expressions)
    - [Boundaries](#boundaries)
  - [Author](#author)

## Regex Components

This expression contains the following
1.	^ and $. 
2.	( )
3.	\d 
4.	{2} 
5.	\d{2} 
6.	(\d{2})? 


### Anchors
	To enforce that the match must span the whole string, we can add the quantifiers ^ and $. 
    1. The caret ^ matches the start of the input string
    2.  the dollar sign $ matches the end of the expression.

### Grouping and Capturing
1. ( Marks the starts of the first subexpression.
2. 	) Marks the ends of the first 
   
### Bracket Expressions
1. 	\d matches any digit character.
2. '-' matches the literal hyphen character.
3. {2} match the first subexpression exactly two times.


### Boundaries
1. \d{2} matches exactly two digits.
2.	(\d{2})? matches exactly two digits. But it’s optional, so the year can contains either two digits or four digits.

## Author

Rene Garcia 

https://github.com/garcia3325
