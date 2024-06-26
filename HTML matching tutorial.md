# HTML matching

In this tutorial, we will be exploring how to utilize the regular expression (regex) to match an HTML tag. Specifically the regex to match a full HTML tag '/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/'. 

## Summary

We will be breaking down the aforementioned regex to further explain each component and how exactly it is able to match an HTML tag. This regex tag covers the following: opening tag, attributes, content, and closing tag.

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
We use anchors '^' to declare postioning within the string, ensuring the string matches the regex.

### Quantifiers
Quantifiers determine how many times a character or group mst be present for an exact match. The regex provided above does so using: 
* matches 0 or more occurrences of the preceding element.
+ matches 1 or more occurrences of the preceding element.

### OR Operator
The '|' operator acts like a logical OR, allowing alternative matches. In our regex, (?:>(.*)<\/\1>|\s+\/>) uses the OR operator to match either a full tag with content or a self-closing tag.

### Character Classes
These match any single set of characters. i.e '[a-z]' -matches any lowercase letter.

### Flags
N/a in this regex.

### Grouping and Capturing
Parentheses () are used for grouping and capturing. In our regex:

([a-z]+) captures the tag name.
([^<]+)* captures attributes.
(?: ... ) is a non-capturing group.
(.*) captures the tag content.

### Bracket Expressions
These will define a character class as mentioned in the earlier section.

### Greedy and Lazy Match
As the names suggest Greedy matches will try to match as much as possible, while lazy matches attempt the opposite. In our regex, .* is greedy and will match as much content as possible until the closing tag.

### Boundaries
Boundaries are not used in this regex. anchors are used instead.

### Back-references
Back-references refer to previously captured groups. \1 refers to the first captured group, ensuring that the closing tag matches the opening tag.

### Look-ahead and Look-behind
These are also not used in this regex, but typically allow for matching a pattern only if it is before or after another pattern.

## Author

This tutorial was created by Patrick Castorena to assist in understanding the regex function for HTML matching. I am new to coding for the most part with 6 months of experience and some projects under my belt available at: https://github.com/PCast71. Feel free to reach out to me with any further questions also at patrickc77hhs@gmail.com!
