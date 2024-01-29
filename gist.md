# Matching an email regex

Regular expressions (regex) serve as potent tools for pattern matching in strings. This guide delves into a regex pattern crafted for identifying email addresses. The email regex is `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`.

## Summary

The regex provided aims to validate and extract components from an email address. It breaks down an email into three main parts: the username, the domain, and the top-level domain (TLD). The pattern ensures that the email adheres to common email format rules.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
- `^`: Anchors the match at the beginning of the string.

- `$`: Anchors the match at the end of the string.
### Quantifiers
- `+` (Plus Quantifier):
    Placed after a character class or a group, it indicates that the preceding character or group must appear one or more times.

- `{2,6}` (Curly Braces Quantifier):
    Written as `{m,n}`, it specifies a range for occurrences. The preceding character or group must appear at least `m` times and at most`n`times.
### Grouping Constructs
- **Username Grouping**: (`[a-z0-9_\.-]+`)
    - This group captures the username part of the email address.
        
- **Domain Grouping**: (`[\da-z\.-]+`)
    - This group captures the domain part of the email address.

- **TLD Grouping**: (`[a-z\.]{2,6}`)
    - This group captures the top-level domain (TLD) part of the email address.
### Bracket Expressions
- **Username Character Class**: `[a-z0-9_\.-]`
- **Domain Character Class**: `[\da-z\.-]`
- **TLD Character Class**: `[a-z\.]`
### Character Classes
- **Username Character Class**: `[a-z0-9_\.-]`

    - This character class allows the following characters for the username:
        - Lowercase letters (a-z).
        - Digits (0-9).
        - Underscore (_).
        - Dot (.).
        - Hyphen (-).

- **Domain Character Class**: `[\da-z\.-]`
    - This character class allows the following characters for the domain:
        - Digits (\d).
        - Lowercase letters (a-z).
        - Dot (.).
        - Hyphen (-).

- **TLD Character Class**: `[a-z\.]`
    - This character class allows the following characters for the top-level domain (TLD):
        - Lowercase letters (a-z).
        - Dot (.).
### Flags
- `i`: (case-insensitive): Makes the regex match case-insensitively, allowing it to match both uppercase and lowercase letters interchangeably.
### Character Escapes
- `\.`: Escapes the dot to match a literal dot.
## Author

**Ronald Martin**
- [Github](https://github.com/RonaldMartin02)
