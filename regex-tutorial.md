# Regex Tutorial

Regex, which is short for regular expression, is a sequence of charactters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patters of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input. 

## Summary

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

This regex validates whether or not the input is an email address. 

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

The anchors used in this regex are `^` and `$`. 
The `^` is used to degine the beginning of the string, and the `$` defines the end of the string. 

### Quantifiers

A quantifier set the limits of the string that your regex matches (or an individual section of the string). They frequently include the minimum and maximum number of characters that the regis is looking for. 

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` 

The quantifiers are the plus `+` operator, `{2,6}`, and `[a-z\.]`. 
The `+` will connect the users email name `+` email service. 
The `{2,6}` will allow a match range of 2-6 characters for the character set of `[a-z\.]`.

### Grouping Constructs

Grouping constructs is done by using parentheses () in the regex. 
In this expression,

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` 

In this expression there are 3 groups.

 `([a-z0-9_\.-]+)` Which is responsible for mating the email string. 

 `([\da-z\.-]+)` Whcih is responsible for matcching the email service.

 `([a-z\.]{2,6})` Which is responsible for (.com/.edu/etc). 

### Bracket Expressions

Anything inside a set of square brackets [ ] represent a range of characters that we want to match. Within the code, there are three bracket expressions: 

`[a-z0-9_\.-]` Which matches any lowercase letters from a-z, and any digit from 0-9. 

`[\da-z\.-]` Which matches any lowercase letters from a-z and the character "."

`[a-z\.]` Which matches any lowercase letters from a-z.
### Character Classes

A character class in a regex defines a set of characters, any one of which can occur in an input string to filfill a match. In the code example, the only character classe is: 

`\d` Which is used to match any digit character. 

## Author
Kalani Mojica
- [Github](https://github.com/mojikalani)
- [LinkedIn](https://www.linkedin.com/in/kalani-mojica-132042206/)
