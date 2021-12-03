# Title (replace with your title)

Hello! My name is Alexander Cooney, For the next few minutes I would love to be your guide through the wonderful world of regex or REGULAR EXPRESSIONS. The are quite bizarre looking at first, as per our example we will come back to time and again through this tutorial /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{3,9})$/

## Summary

As we saw above a regular expression, which we will be calling regex for short, can look quite daunting at first, but it is simply a way of matching or validating strings such as email addresses. So take a few moments to get acquainted with regex with the documentation I've written below as an introduction to the world of regex. 

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
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
An Anchor is a symbol indicating the beginning or end of a regular expression string. The Carrot symbol as shown here ^ indicates the beginning, and the Dollar Sign symbol $ indicates the end of the regular expression. Our example email /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{3,9})$/  we can more clearly see this process. Again, the carrot ^ notating the start and dollar sign $ notating the end of the email in between the two forward slashes. 
### Quantifiers
Quantifiers are notated towards the end of the Regex string with Curly Brackets {} , these numbers describe how many characters from the earlier regex must be a match. Per our example /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{3,9})$/ this refers to the 3 and 9, meaning we must have a minimum of 3 and max of of the preceding characters requested to be a match.
### OR Operator
For an OR operator we us the | symbol. It is used as a logic operator in a Boolean form. say we had a list of three people Alex|steve|bryan, the or operator would be saying choose alex or steve or bryan for this task. In this way we can see how many or if any characters match a certain list of other characters. 

### Character Classes
Character Classes map out what characters will be a match for the Regex expression, these characters are are placed in [] brackets. The easiest way to learn is by observing our Regex sample /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{3,9})$/  There are a few examples of character classes in our email expression. [a-z0-9_.-], [\da-z.-], and [a-z.] respectively. The first one is saying to accept all lowercase letters a-z, all numbers 0-9, and the specific special characters "." and "-" he second express adds a "da-z". The d stands for all digits in addition to the other characters in the expression. The third expression accepts characters that are lowercase a-z and the special character "."
### Flags

Flags in regular expressions are optional parameters that can alter the behavior or searching or matching the expressions. Flags come in a wide array of types, but some common ones are the i for Ignore casing, g for Global, making the expression search for all occurrences, the s for Dot All making the . or wild character match newlines as well, m for Multiline, making the boundary characters ^ and $ match the beginning and ending of every single line instead of the beginning and ending of the whole string. A quick google search for regex flags will give you large databases describing each flags function.

### Grouping and Capturing
Grouping and Capturing are done inside Parenthesis (). Just as the name suggests, they group and divide the regex expression. So if we had an email with an @ symbol say alex@gmail.com , we could break up our regular expression with (). Again, the best way to learn is by demonstration. If we look at our example once again, /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{3,9})$/, we see that we have three groups, or sets of parenthesis. The first group comes before the @ symbol, the second group comes after the @ symbol but before the period, and the last group comes after the period. This is obviously useful when dealing with constraints of email address formats. 
### Bracket Expressions

### Greedy and Lazy Match
Greedy and Lazy are different ways of matching the desired regex expressions and are polar opposites of each other. Greedy matches are trying to match the longest string possible, whereas the lazy matches are trying to match the shortest match possible based on the criteria given. An example of a greedy match is when the plus sign "+" is used. The plus sign means match one or more of the qualifying characters. This is found in two of our groups in our email example, /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{3,9})$/ To make it a lazy expression a question mark "?" needs to be added after the plus sign. As we can see our example is looking for a greedy match. 

### Boundaries
Boundaries, or word boundaries are ways of demarking where one type of character is being used and another type of character is being used. 


### Back-references
back-references are regular expression commands which refer to a previous part of the matched regular expression. Back-references are specified with backslash \ and a single digit. 

## Author

My name is Alexander Cooney, I am attending the University of Texas coding boot camp. I have always had a great interest in technologies and am extremely happy with how much I have learned thus far. My github account is https://github.com/AFC2134
