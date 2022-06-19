# REGEX Tutorial: 

 URL regex: URL regular expressions can b used o verify if a string has a valid URL format as well as to extract an URL from a string.



## Summary
This regex validates a url which should include http or https.
```
https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()!@:%_\+.~#?&\/\/=]*)
```



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

# Regex Components

## Anchors

Anchors have special meaning in regular expressions.  They do not match any character.  They match a position before or after characters.

- ```^``` - The caret anchor matches the beginning of the text.
- ```$``` - The dollar anchor matches the end of the text.

## Quantifiers

Quantifiers match a number of instances of a character, group or character class in a string.

- ```?``` - The quantifier ? searches the pattern zero or one time.  
- ```*```- The quantifier * searches the pattern zero or more times.
- ```+```- The quantifier + searches for the pattern one or more times.

## OR Operator

The purpose of an OR operator is to match the characters on the left or right of the operator, essentially serving as an or, as in and/or. Using the | as in k|K would match either m or an M from the string. 
If we had used ```https?:\/\/(www\.)?[\d-r|R it would search for r or R```

## Character Classes

A character class allows you to match any symbol from a certain character set.  It is also called a character set.

- ```\d``` - matches a single digit.
- ```\s``` - matches any whitespace such as a space, a tab, and newlines.
- ```\D``` - matches any character except digits.
- ```\S``` - matches any character except whitespace. (for example, a letter)

## Flags

Regular expressions may have flags that affect the search.  Flags are used at the end of the Regex, after the closing slash. 

There are only 6 of them
- ```i```- With this flag the search is case-insensitive.  There is no differance between A or a.
- ```g```- With this flag the search looks for all matches, without it only the first match is returned
- ```m```- Multiline.  Makes the boundary characters ^ and $ match beginning and end of every line
- ```s```- Enables "dotall" mode.  allows a dot . to match newline character /n.
- ```u```- Enables full Unicode support.  This flag enables correct processing of surrogate pairs.
- ```y```- "Sticky" mode.  Searching at the exact position in the text.

An example of a flag is shown here.
```https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()!@:%_\+.~#?&\/\/=]*)g```

## Grouping and Capturing

A part of a pattern can be enclosed in parentheses.  This is called a 'capturing group'  (...)

This has two effects:
- It allows to get a part of the match as a separate iten in the result array.
- If a quantifier is added after the parentheses, it applies to the parentheses as a whole.
## Bracket Expressions

Several characters or character classes inside square brackets mean to "search for any character among given".  [....]

## Greedy and Lazy Match

By default, quantifiers use the greedy mode for matching.  To transform a greedy quantifier into a lazy (non-greedy) quantifer you add an extra ? to it.

- Greedy -```*```-
- Lazy -```*?```-

## Boundaries

Boundaries are similar to anchors.  Where anchors use the ^ and $ symbols, boundaries have the \b.  It matches a position that is called a 'word boundary'.

The following are qualified as word boundaries.
- Before the first characher in a string if the first character is a word character
- After the last character in a string if the last character is a word character.
- Between two characters in a string if one is a word character and the other is not.

## Back-references

Backrefernce is a way to repeat a capturing group. For example the ```([A-Za-z])[0-9]\1. The group '([A-Za-z])' is back-referenced as \\1.```

## Look-ahead and Look-behind

Lookahead and lookbehind, collectively called “lookaround”, are zero-length assertions just like the start and end of line, and start and end of word anchors. The difference is that lookaround actually matches characters, but then gives up the match, returning only the result: match or no match. That is why they are called “assertions”. They do not consume characters in the string, but only assert whether a match is possible or not. Lookaround allows you to create regular expressions that are impossible to create without them.

# Author
Inglish Foust is a student at Butler University enrolled in The Trilogy Bootcamp.  She is currently living in Indiana and has hopes and dreams for her future in the web development world.

* [Inglish's GitHub](https://github.com/Inglish2022)


