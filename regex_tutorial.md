# Regex Tutorial

Regular expressions, commonly known as regex, are powerful tools for pattern matching and text manipulation. They are used in various programming languages and tools to search, match, and manage strings based on specific patterns. Whether you're cleaning data, validating input, or parsing logs, regex can simplify your tasks significantly.

## Summary

In this tutorial, we will explore the essential components of regular expressions, including anchors, quantifiers, grouping constructs, bracket expressions, character classes, the OR operator, flags, and character escapes. By the end of this tutorial, you'll have a solid understanding of how to construct and use regex patterns effectively.

Example regex: `^(\d{3})-(\d{2})-(\d{4})$`

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

Anchors are used to specify the position within a string where a match must occur. The two most common anchors are:

- `^` - Matches the start of a string.
- `$` - Matches the end of a string.

Example:
- `^Hello` matches "Hello" at the start of a string.
- `world$` matches "world" at the end of a string.

### Quantifiers

Quantifiers define the number of times an element can occur in a regex pattern. Common quantifiers include:

- `*` - Matches 0 or more occurrences.
- `+` - Matches 1 or more occurrences.
- `?` - Matches 0 or 1 occurrence.
- `{n}` - Matches exactly n occurrences.
- `{n,}` - Matches n or more occurrences.
- `{n,m}` - Matches between n and m occurrences.

Example:
- `a*` matches "a", "aa", and "" (empty string).
- `a{3}` matches "aaa".

### Grouping Constructs

Grouping constructs allow you to group parts of a regex pattern together. This is useful for applying quantifiers to multiple elements or capturing matches for later use.

- `()` - Capturing group.
- `(?:)` - Non-capturing group.

Example:
- `(abc)+` matches "abc", "abcabc", etc.
- `(?:abc)+` also matches "abc", "abcabc", etc., but does not capture the groups.

### Bracket Expressions

Bracket expressions, or character sets, match any one of the characters inside the brackets.

- `[abc]` - Matches any one of "a", "b", or "c".
- `[^abc]` - Matches any character except "a", "b", or "c".

Example:
- `[0-9]` matches any digit.
- `[a-zA-Z]` matches any letter.

### Character Classes

Character classes provide a way to match a specific set of characters.

- `\d` - Matches any digit (equivalent to `[0-9]`).
- `\D` - Matches any non-digit.
- `\w` - Matches any word character (alphanumeric and underscore).
- `\W` - Matches any non-word character.
- `\s` - Matches any whitespace character.
- `\S` - Matches any non-whitespace character.

Example:
- `\d{3}` matches exactly three digits.

### The OR Operator

The OR operator `|` allows you to match one pattern or another.

Example:
- `cat|dog` matches "cat" or "dog".

### Flags

Flags modify the behavior of a regex pattern. Common flags include:

- `i` - Case-insensitive matching.
- `m` - Multiline mode.
- `s` - Dotall mode (dot matches newlines).
- `g` - Global match (find all matches rather than stopping after the first match).

Example:
- `/hello/i` matches "hello" and "Hello".

### Character Escapes

Character escapes allow you to match characters that have special meaning in regex or to specify characters by their Unicode code points.

- `\.` - Matches a literal dot.
- `\\` - Matches a literal backslash.
- `\u00A9` - Matches the Unicode character ©.

Example:
- `3\+3=6` matches "3+3=6".

## Author

This tutorial was written by Oscar Osorio
https://github.com/Osorio-333 
