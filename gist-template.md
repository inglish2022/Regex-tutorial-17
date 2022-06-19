# REGEX Tutorial: 

 URL regex: URL regular expressions can b used o verify if a string has a valid URL format as well as to extract an URL from a string.



## Summary
This regex validates a url which should include http or https.

https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()!@:%_\+.~#?&\/\/=]*)


Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

## Anchors

Anchors have special meaning in regular expressions.  They do not match any character.  They match a position before or after characters.

- ^ - The caret anchor matches the beginning of the text.
- $ - The dollar anchor matches the end of the text.

## Quantifiers

Quantifiers match a number of instances of a character, group or character class in a string.

- ? - The quantifier ? searches the pattern zero or one time.  
- '*'- The quantifier * searches the pattern zero or more times.
-

## OR Operator

The purpose of an OR operator is to match the characters on the left or right of the operator, essentially serving as an or, as in and/or. Using the | as in k|K would match either m or an M from the string. 
If we had used https?:\/\/(www\.)?[\d-r|R it would search for r or R

## Character Classes

A character class allows you to match any symbol from a certain character set.  It is also called a character set.

- \d - matches a single digit.
- \s - matches any whitespace such as a space, a tab, and newlines.
- \D - matches any character except digits.
- \S - matches any character except whitespace. (for example, a letter)

## Flags



## Grouping and Capturing

## Bracket Expressions

## Greedy and Lazy Match

By default, quantifiers use the greedy mode for matching.  To transform a greedy quantifier into a lazy (non-greedy) quantifer you add an extra ? to it.

- Greedy -*-
- Lazy -*?-

## Boundaries

Boundaries are similar to anchors.  Where anchors use the ^ and $ symbols, boundaries have the \b.  It matches a position that is called a 'word boundary'.

The following are qualified as word boundaries.
- Before the first characher in a string if the first character is a word character
- After the last character in a string if the last character is a word character.
- Between two characters in a string if one is a word character and the other is not.

## Back-references

## Look-ahead and Look-behind

# Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
