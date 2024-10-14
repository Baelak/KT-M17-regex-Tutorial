# REGEX Turtorial - Matching an Email

## Gist URL - https://gist.github.com/Baelak/7ad53f289e4092d1359461e8d3b6e7ff

## /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

In this tutorial, we'll explore the regular expression used for matching email addresses. Understanding how regex patterns work is essential for validating user input, particularly in web development. This regex ensures that the email format adheres to common standards, helping to filter out invalid addresses and improve data quality.

## Summary

The regex pattern we'll be breaking down is /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. This regex is designed to match email addresses, ensuring they begin with a valid string before the @ symbol, followed by a valid domain name. Each part of the regex plays a crucial role in defining what constitutes a valid email address.

## Table of Contents

- [Anchors](#anchors)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors
The regex starts with a caret (^) and ends with a dollar sign ($). These anchors specify that the match must occur at the beginning and the end of the string, ensuring that the entire string is validated as an email address.

### Character Classes
The regex includes character classes defined by brackets, such as [a-z0-9_\.-] and [a-z\.]. These classes allow the regex to match any single character from the specified set. The first class matches lowercase letters, digits, underscores, periods, and hyphens, while the second class matches lowercase letters and periods.

### Grouping and Capturing
The parentheses () in the regex create capture groups. The first group ([a-z0-9_\.-]+) captures the local part of the email, the second group ([\da-z\.-]+) captures the domain name, and the third group ([a-z\.]{2,6}) captures the top-level domain. This allows for further processing or validation of each segment of the email.

### Bracket Expressions
Bracket expressions define sets of characters that can match a single position in the input string. In this regex, [a-z0-9_\.-] specifies valid characters for the local part, and [a-z\.] specifies valid characters for the top-level domain.

### Greedy and Lazy Match
This regex uses greedy matching, which means it will match as many characters as possible. For instance, in the pattern ([a-z0-9_\.-]+), it will match all valid characters until it encounters the @ symbol.

## Author

Hi I am Kaleab. I am a GWU Fullstack Developer Bootcamp student and I created this tutorial as part of an assignement. Feel free to visit my [GitHub profile]([url](https://github.com/Baelak?tab=repositories)) for more projects. 😊

 <div style="display: flex; justify-content: center; border-bottom: 1px solid #ddd; padding-bottom: 10px; margin-bottom: 20px;">
  <img src="./Develop/generatedQR.png" alt="Logo" style="max-height: 200px; max-width: 200px;">
</div>