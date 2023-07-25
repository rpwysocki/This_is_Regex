# This_is_Regex

This is a desciption and tutorial of regex expression.

## Summary

The regex covered here is for a URL. `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/` is the regex that will be broken down to explain each sections purpose.

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

### Anchors
    Anchors are the beginning and end of a string of characters.
    '^': This symbol denotes the start of the string.
    '$': This symbol denotes the end of the string.

### Quantifiers
    Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found.
    ':\/\/' matches the exact characters "://"
    The + indicates that one or more of these characters should be matched
    ([a-z\.]{2,6}) allows two to six lowercase letters or dots

### OR Operator
    The "or" operator is designated by the "|" pipe character.
    It is not used in this regex example.

### Character Classes
    A character class. Matches any one of the enclosed characters. You can specify a range of characters by using a hyphen, but if the hyphen appears as the first or last character enclosed in the square brackets, it is taken as a literal hyphen to be included in the character class as a normal character.
    ([\da-z\.-]+): This part matches the domain name, which can contain lowercase letters, digits, dots, and hyphens


### Flags
    A flag is an optional parameter to a regex that modifies its behavior of searching
    A flag changes the default searching behavior of a regular expression. It makes a regex search in a different way
    A flag is denoted using a single lowercase alphabetic character

### Grouping and Capturing
    Groups group multiple patterns as a whole, and capturing groups provide extra submatch information when using a regular expression pattern to match against a string


### Bracket Expressions
    A bracket expression (an expression enclosed in square brackets, "[]" ) is an regex that shall match a specific set of single characters, and may match a specific set of multi-character collating elements, based on the non-empty set of list expressions contained in the bracket expression


### Greedy and Lazy Match
    - In a greedy match for each position in the string, the pattern is matched at that position
    In case there is not any match, it is necessary to go to the next position
    - In a lazy match it is the opposite of the greedy match
    It considers repeating a minimal number of times, it can be enabled by using a question mark '?' after the quantifier

### Boundaries
     A word boundary "\b" detects a position where one side is such a character, and the other is not

### Back-references
    Back-references are regular expression commands which refer to a previous part of the matched regular expression
    Back-references are specified with backslash and a single digit " \1 "

### Look-ahead and Look-behind
    Lookahead and lookbehind (commonly referred to as “lookaround”) are useful when we'd like to match something depending on the context before/after it
    - Lookahead the syntax is: X(?=Y), it means "look for X, but match only if followed by Y". There may be any pattern instead of X and Y
    - Lookbehind is similar, but it looks behind. That is, it allows to match a pattern only if there’s something before it.
        Positive lookbehind: (?<=Y)X, matches X, but only if there’s Y before it.
        Negative lookbehind: (?<!Y)X, matches X, but only if there’s no Y before it.

## Author

Brought to you by: Ryan Wysocki

Github profile: https://github.com/rpwysocki
