# Ivas Regex Tutorial

Use this tutorial to help you search for information in your code!

## Summary

A regular expression is a sequence of characters that defines a search pattern in a search pattern for text.

## Table of Contents

- [Regex Components](#regex-components)
- [Anchors](#anchors)
- [Bracket Expressions](#bracket-expressions)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)
- [Grouping Constructs](#grouping-constructs)

## Regex Components

Litteral character VS Meta Character

We use expressions when we are trying to find a certain sequence of characters through a search pattern. For example if we are searching for a phone number.
We can use meta character d for digit (/d/d/d-d/d/d-/d/d/d/d). We enter this into the search and use regex ._ to allow us to search for any character.
. -> any character _ is a quantifier meaning 0 or more. Syntax highlighting will match those characters for you.

### Anchors

Anchors are the characters (^) and ($).

- ^ represents a string that begins with the characters that follow it.
- $ represents a string that ends with characters that go before it.

### Bracket Expressions

Bracket Expressions represent a range of characters we want to match. This range of outline the characters we want to include and is also known as the positive character group. For example [0-9] The string can only contain any numnber between 0-9.

### Quantifiers

Now what are we looking for inside these brackets? Quantifiers set limits on the string that your regex matches. Quantifiers will match as many instances of certain patterns as possible.

- - Matches the pattern 0 or more times
    +- Matches the pattern 1 or more times
    ?- Matches the pattern 0 or 1 times
    {}- Provide 3 different ways to set limits:

1. { n } - Matches the pattern exactly n times
2. { n, x } - Matches the pattern at least n times
3. { n, x } - Matches the patern from a minimun of n times to a maxmimum x times

Add ? to the end and it will match as many instances as possible

### Character Classes

### The OR Operator

### Flags

### Character Escapes

### Grouping Constructs

### Bracket Expressions

## Author

I'm a new web developer currently living in Toronto. My background is in Fashion and Automotive. I like going on adventures, working on my car and i'm also a bartender. Follow my journey at https://github.com/Iva416
