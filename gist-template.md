# Title (replace with your title)

In this tutorial, we will be exploring how to utilize the regular expression (regex) to matchc an HTML tag. Specifically the regex to match a full HTML tag '/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/'. 

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

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
