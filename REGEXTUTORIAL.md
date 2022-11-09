# Ivas Regex Tutorial

Use this tutorial to help you learn about Regex and help you search for information in your code!

## Summary

Regex will help you search for chracters and values in your code.

## Table of Contents

- [Regex Components](#regex-components)
- [Anchors](#anchors)
- [Bracket Expressions](#bracket-expressions)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

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

    *- Matches the pattern 0 or more times
    +- Matches the pattern 1 or more times
    ?- Matches the pattern 0 or 1 times
    {}- Provide 3 different ways to set limits:

1. { n } - Matches the pattern exactly n times
2. { n, x } - Matches the pattern at least n times
3. { n, x } - Matches the patern from a minimun of n times to a maxmimum x times

Add ? to the end and it will match as many instances as possible

### Character Classes

In regex character classes define a set of characters in that are in an input string to find a match. Bracket expressions are an example of a character class.
Here are some examples:

\d - Matches any difit this class is the bracket expression [0-9]
\w - Matches any alphanumeric character from the latin alphabet this class is equivelent to the bracket expression [A-Za-Z0-9_]

### The OR Operator

The OR operator (|)

The OR Operator allows us to search for logic outside of a bracket expression or within the grouping of a contruct or different constructs.

For example [abc] if written as (a|b|c)
We take the original expression (abc):(xyz)
Then use the OR operator (a|b|c):(x|y|z)

This will return matching strings "abc:xyz" and "acb:xyz" as well as "a:z"
but "xyz:abc" would not.

### Flags

Regex must be wrapped in slash characters. The exeption to this rule is a component known as flags. They are placed at the end of a regec after the second slash for added functionality and or limits.

For example:

g- Global search: the regex tests all possible matches in a string
i- Case insensitive search: will ignore case to find matches
m- Multi-line search: a mutli-line input string will be treated as multiple lines

### Character Escapes

By adding a back slash with a curly brace (/{) tells regex to look for the open curly brace character insead of the beginning to define the quantifier. This is important when we are looking for strings with the same components of a regex.

## Author

I'm a new web developer currently living in Toronto. My background is in Fashion and Automotive. I like going on adventures, working on my car and i'm also a bartender. Follow my journey at https://github.com/Iva416
