# Title: Regex Tutorial - Matching a Social Security Number (SSN)

Introduction:
Welcome to this tutorial on understanding and using regular expressions to match Social Security Numbers (SSNs). In this tutorial, we will break down the regex components and explain how they work to validate SSN patterns.

## Summary

The regex /^\d{3}-\d{2}-\d{4}$/ is designed to validate the standard format of a Social Security Number, such as "123-45-6789". We will explore each part of this regex and understand its purpose and functionality.
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
Anchors are used to match the position of the SSN pattern within a string.
^ - The caret symbol is used to match the beginning of the string. In this case, the SSN pattern must be at the beginning of the string.

### Quantifiers
Quantifiers specify the exact number of digits required for each part of the SSN.
\d{3}-\d{2}-\d{4} - The \d is a shorthand for the character class [0-9], which matches any digit. The {3} specifies that the SSN must contain exactly 3 digits. The - matches the hyphen character. The \d{2} specifies that the SSN must contain exactly 2 digits. The \d{4} specifies that the SSN must contain exactly 4 digits.

### Character Classes
 Character classes define the allowed range of characters in the SSN pattern.
 \d - The \d is a shorthand for the character class [0-9], which matches any digit. The SSN pattern must contain exactly 3 digits, followed by a hyphen, followed by exactly 2 digits, followed by a hyphen, followed by exactly 4 digits.

### Grouping and Capturing
Grouping allows capturing parts of the SSN pattern as separate entities.
(\d{3})-(\d{2})-(\d{4}) - The parentheses () are used to group and capture the SSN pattern as three separate entities. The first group (\d{3}) captures the first 3 digits of the SSN. The second group (\d{2}) captures the next 2 digits of the SSN. The third group (\d{4}) captures the last 4 digits of the SSN.

## Author
Hi, I'm Ryan, the author of this tutorial. I have a passion for regular expressions and simplifying complex patterns. You can find more of my work using my Github username whixh is rslaughter12.

If you have any further questions, feel free to ask!
