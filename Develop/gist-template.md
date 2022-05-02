# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

The following code will be used throughout the lesson to demonstrate how to utilize the various components of regex. Matching emails may be done with the code below. This code may be used to validate an email to ensure that it is formatted correctly.

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
The anchor is what starts and ends the regular expression. 
In the matching email code, 

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`, 

the anchors are the `^` and the `$`. This code specifically is saying that we are looking for something that starts with 

`^([a-z0-9_\.-]+)` 

we will define what everything inside the parentheses later in this tutorial, but what the anchor means is that if we are to find a match it has follow those initial guidelines. It also has to end with 

`.([a-z\.]{2,6})$`.


So, it must start and end with the given parameters within the code. If it does not, then it is not a match. 
### Quantifiers
A quantifier is used to indicate how many times a certain character or set of characters must appear in order for a match to occur. For example, if we used the regex 'xyz+' in our regex, it would match any text xy followed by at least one z. So, let's have a look at our code for email matching:

`([a-z0-9_\.-]+)`

Any string containing the letters a-z, 0-9, _,., or - will be matched. The quantifier '+' indicates that at least one of these must be present for a match to be made.
### OR Operator
Although it is not present in the code for the stated matching email code, we will examine the following code for matching a hex code in order to discuss the OR Operator.

`/^#?

([a-f0-9]{6}|[a-f0-9]{3})

$/`

This is a regex that uses the OR Operator to match a hex code.
This will match where it begins with a '#,' which must come first, followed by one of the following:

'[a-f0-9]6' will match a 6-character string containing a-f letters and 0-9 numerals.

OR Operator '|'

It will match a 3-character long string containing a-f letters and 0-9 numbers, such as '[a-f0-9]3'.

### Character Classes
\d is present in the given matching email code and what it will match a single letter character, a-z, after the @ sign in the email address. Basically ensuring that a letter is matched after the @ in the email and not a number or special character.
### Flags
There is no regex flag in the matching email code used in this tutorial. An example of a regular expression is as follows:

/regex/

The slashes denote the start and end of the regular expression, respectively. A flag can be used after the slash to offer further instructions for our matching. The following are the flags:

The letter g stands for "global," and it allows you to match all instances of a string that fit the regular expression's rules.
The letter m stands for "multiline," which implies that instead of searching the full text, it will search line by line.
The letter I, which stands for "insensitive," makes the regular expression case-insensitive, which means that capital and lower-case letters have no bearing on matching.

### Grouping and Capturing

Continuing with the email matching code:

`/^([a-z0-9_\.-]+)

@([\da-z\.-]+)\.([a-z\.]{2,6})

$/`

We could talk about capturing and grouping.

([a-z0-9_.-]+) is the first group that appears in our regex. This must be true before proceeding to "match" the following section of the code.
'([da-z.-]+)' is the second group that appears in our regex. In our regex, the third group is ([a-z.]2,6).

Before moving on to the next group, we must make certain that we are adhering to the prior group's requirements.
### Bracket Expressions



### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)