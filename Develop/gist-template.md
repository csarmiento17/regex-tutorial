# Regex Tutorial: Matching a URL

This tutorial will show how to create a regex to check if the URL is a valid pattern.

## Summary

The code below is a regex pattern to check for a valid URL.

```
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]_)_\/?$/
```

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

- `^` - Start of string, or start of line in multi-line pattern
- `$` - End of string, or end of line in multi-line pattern

### Quantifiers

In our sample regex, we used 2 Quantifiers, `?` and `+`. The `(https?:\/\/)?` quantifier should match 0 or 1 occurence only while `([\da-z\.-]+)` quantifier matches any string that contains one or more occurrences.

### Character Classes

- `\d` - matches a single character that is a digit
- `\w` - matches a word character (alphanumeric character plus underscore)

Character classes distinguish kinds of characters such as letters and digits. This `([a-z\.]{2,6})` character class checks for for small letters from `a to z` at least two to six characters of the preceding string.

### Grouping and Capturing

This operator is very useful when we need to extract information from strings.

- `(https?:\/\/)` - this sample grouping creates a value of `https://`

### Bracket Expressions

- `[\/\w \.-]` - matches a word character (alphanumeric character plus underscore)

### Greedy and Lazy Match

The quantifiers `*, +, {}` are greedy operators, so they expand the match as far as they can through the provided text.

## Author

I'm a Front-End Engineer who's currently studying Full-Stack Development. Checkout out my [Github Profile](https://github.com/csarmiento17).
