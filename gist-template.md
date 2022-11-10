# Regex Tutorial: Matching an Email

## Definition
**Regular expressions**, or **regex**, are used to extract information from any text by searching for one or more matches of a specific search pattern. They can be used in almost any programming language including JavaScript, Java, Python, Ruby, and many others. 

## Summary
In this tutorial, I will break down the following regex for *matching an email*: <br>
```
^([a-zA-Z0-9._%-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,6})*$
```
This is usually used to validate an email address. An example of this would be if a user is filling out a form online or an inquirer program in Node.js. This regex would be used to make sure an email address is entered when one is ask for. 

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
The email regex uses the anchors `^` and `$`. The caret, `^`, denotes the start of the string and the `$` denotes the end of the string. 

### Quantifiers
Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. The quantifier `+` matches one or more times. The `+` is known as a *greedy operator* because it will match as many instances as possible. In the first instance of `+`, it is looking for one or more characters that satisfy the requirements of `[a-z0-9_\.-]` and later looks for one or more characters in `[\da-z\.-]`. The `{2, 6}` at the end of the regex means that there are between 2 and 6 characters in the group `[a-z\.]`.


### OR Operator
The `[]` OR operator is used in this regex. For example, `[a-z0-9_\.-]` means letters `a-z`, numbers `0-9`, `_`, `.`, or `-`. The `\` is used to denote a literal `.` instead of the usual meaning of `.` which is "any character". 

### Character Classes
The email regex uses the character class `\d` which denotes any digit character `0-9`. The backslash, or `\`, indicates tte character class which is distinct from a plain letter `d`.

### Flags
The regex is enclosed bb two forward slash, or `/`, characters. These come before the caret, `^`, which opens the regex, and after the dollar sign, `$`, which closes the regex. Flags that can be used include `g` for global search, `i` for case sensitive search, and `m` for multiline search. These would come after the closing `/`.

### Grouping and Capturing
Parenthesis, `()` are used to group parts of a regular expression together. In terms of the email regex, the username would be part of one group; the provider/domain name (for example, gmail) would be another group; and finally, the extension (ex. .com, .net, etc.) would be the last group. 

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author
Trae Valdez - Funeral Empire, Inc.<br>
[Github](http://www.github.com/traevaldez)