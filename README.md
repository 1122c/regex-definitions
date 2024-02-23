# regex-definitions

[Link to Regex Tutorial Gist]([URL](https://gist.github.com/1122c/261a4db124b058b70a281bc43b892a34)https://gist.github.com/1122c/261a4db124b058b70a281bc43b892a34)

# Regex Tutorial

A regex, which is short for regular expression, is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input.

## Summary

For example, the following regular expression can be used to verify that user input is a valid email address:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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

Regular expressions (regex) are powerful tools for matching patterns in text. Here's a brief overview of their key components:

### Anchors
In regex anchors are symbols that denote the beginning and end of a search type. 

For example, in our email regex, the ^ symbol denotes the beginning of a string, while the $ symbol indicates the end of that same string.

### Quantifiers

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. They include:

- * (zero or more)
- + (one or more)
- ? (zero or one)
- {n} (exactly n times)
- {n,} (at least n times)
- {n,m} (between n and m times, inclusive)

### OR Operator

The OR operator is represented by |. It matches the expression before or after the |. It can be used within a group (a|b) to match either a or b.

### Character Classes

Character classes match any character from a specific set and are denoted by brackets []. For example, [abc] matches any single character a, b, or c. Special character classes include:

- \d matches any digit (equivalent to [0-9]).
- \w matches any word character (equivalent to [a-zA-Z0-9_]).
- \s matches any whitespace character (spaces, tabs, line breaks).

### Flags

Flags modify the behavior of the regex pattern. They are appended to the end of the pattern. Common flags include:

- g (global search)
- i (case insensitive search)
- m (multi-line search)
- u (unicode support)
- s (allows . to match newline characters)
  

### Grouping and Capturing

Parentheses () are used to group parts of a regex together, and to capture the content matched by that part of the regex. This allows you to extract information from strings or to apply quantifiers to entire groups.


### Bracket Expressions

Bracket expressions are similar to character classes but are more specific. They allow you to include a range of characters [a-z], exclude specific characters [^a-z], or specify a set of characters [aeiou] that can match.


### Greedy and Lazy Match

Quantifiers in regex are greedy by default, meaning they match as many occurrences of a pattern as possible. The lazy (or reluctant) versions of quantifiers attempt to match as few occurrences as possible. They are made lazy by adding a ? after the quantifier, e.g., *?, +?, ??, {n,m}?.


### Boundaries

Word boundaries \b and non-word boundaries \B are used to match positions where a word character is next to a non-word character, and vice versa. They are useful for whole word searches.


### Back-references

Back-references match the same text as previously matched by a capturing group. They are denoted by \n, where n is the number of the capturing group.


### Look-ahead and Look-behind

Look-ahead and look-behind assertions are zero-length assertions that match a position based on what follows ((?=...) for look-ahead) or precedes ((?<=...) for look-behind) the current position without including it in the match.

- Positive look-ahead (?=regex) matches a group after the main expression without including it in the result.
- Negative look-ahead (?!regex) matches if the group does not occur after the main expression.
- Positive look-behind (?<=regex) matches a group before the main expression without including it in the result.
- Negative look-behind (?<!regex) matches if the group does not occur before the main expression.
  

## Author

Rachel, certification of completion candidate at Northwestern University, March 2024
