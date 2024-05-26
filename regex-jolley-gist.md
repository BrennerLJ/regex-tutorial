# Regex: How It Works

In this tutorial, I'm going to teach you about Regex.

## Summary

I will teach you how Regex works using telephone numbers.

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

Special characters in expressions that assert specific positions in a string without matching any actual characters. They ensure that pattern matches at the beginning or ending of a string.

### Quantifiers

Specify the number of times a pattern should be matched. They can be greedy or lazy.

### OR Operator

Used to match one pattern or another. Represented with the '|' symbol. Ex. Matching either "cat" or "dog". 

### Character Classes

Used to match a set of characters. Square brackets are used, you can list specific characters, ranges of characters, or a combination of both. Character classes in regular expressions to match phone numbers can help you find different formats. Ex. `/^(\+1\s?)?(\(?\d{3}\)?[\s.-]?)?\d{3}[\s.-]?\d{4}$/`
// Valid phone numbers
// 123-456-7890
// 123.456.7890
// 123-456-7890
// 1234567890
// (123) 456-7890
// +1 (123) 456-7890

### Flags

Modifiers that can be added to the regex to change its behavior. For example, a `g` flag can be added to find all instances in the text, `m` flag can be used if you have a multiline string where phone numbers appear at the beginning or end of lines.

### Grouping and Capturing

Used to group parts of a pattern together and capture them for later use. Can be used to extract certain parts of a phone number, like area code.

### Bracket Expressions

Used to match a set of characters, such as digits and separators. 

### Greedy and Lazy Match

Greedy match tries to match as many characters as possible, of a pattern, while lazy match tries to match as few characters as possible. Examples of greedy quantifiers: `*`: matches 0 or more occurances, `+`: matches 1 or more occurances. Lazy quantifiers are created by appending a `?` to the greedy  quantifier. Ex. `*?`: matches 0 or more occurances (as few as possible), or `+?`: matches 1 or more occurances (as few as possible).

### Boundaries

Used to match specific positions in a string rather than matching actual characters. Types of boundaries include, 1. Word Boundaries: `\b` and `\B`, 2. Line Boundaries: `^` and `$`, and 3. String Boundaries: `\A`, `\Z`, and `\z`.

### Back-references

Used to match the same text that was matched by a previous group.

### Look-ahead and Look-behind

Used to assert that a pattern is or is not present without including it in the match.

## Author

Hi! My name is Brenner, I have learned a lot about coding and hope this tutorial helps you learn something new! Here is my Github page: https://github.com/BrennerLJ/regex-tutorial/blob/main/regex-jolley-gist.md
