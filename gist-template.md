# Title (replace with your title)

This in and introductory explanation for what a regex is, and specifically how a regex to verify an email address works. This explanation will be broken into separate sections, each explaining a different part of the regular expression. You can click on the different links in the table of contents to quickly jump to the explanations for those parts.

## Summary

The regex explained in this gist, is the regex used to verify an email address, as shown here: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
This expression is broken into three main sections, each encased with parenthesis. The first verifies the beginning of the email, which is then separated by the @ symbol. The next verifies the domain, like gmail, ended with a dot or a slash, then the last part verifies the ".com", or ".net" part.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)

## Regex Components

### Anchors
The anchor denotes the start of the string / expression, it is represented by the "^" symbol.

### Quantifiers
Quantifiers are symbols that denote how many times characters should appear. In this expression, the quantifier is the "+" symbol, which means that these characters should appear at least 1 time, but can appear more than once.

### Character Classes
A character class is a set of characters within square brackets, "[]". It basically means that the characters inputted by the user will match at least 1 of the characters withing the brackets. Basically like saying that the given input can include any of the characters within the brackets. It has to at least have one of them, but you can have multiple if you want.

For example, in the first class of the expression, it's saying that this part of your input can include lowercase characters from a-z, numbers from 0-9, an underscore, slash, dot, and / or dash.

The second class is similar in that it can include character from a-z, a slash, dot, or dash.

Lastly, the last class can also include characters from a-z, a slash, or a dot. 

### Grouping and Capturing
Capture groups refer to parts of an expression inside parentheses. You can name them, but you don't have to, and their purpose is to reference different parts of the expression based on the whole. Basically it's a container or section of an expression that matches values in a group.

This expression has 3 groups, namely the first part of the email, for example, if my email was "student123@gmail.com", the first group would be for the "student123" part. The second group would be for the "gmail" part, and the last group would be for the ".com" part.

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
