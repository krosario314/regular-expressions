# Regex Matching HEX Values
Regular expressions also known as Regex, are search patterns defined into a specific sequence of characters. This technical tutorial explains and breaks down the functionality of the regex for matching HEX values. 
#
## Summary
This technical tutorial will be explaining and breaking down components within the regular expression used to match HEX values which is shown in the snippet below. Hexadecimal code is a system that accurately describes a specific color to your computer. The hexadecimal code starts with a '#' and contains 6-digits.

Regex for matching HEX values

```
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
```
#
## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
#
## Regex Components
#
## Anchors

Anchors are used to match a position anywhere within the characters. Anchors such as  ``` ^ ```  and  ```$```  can be used to pinpoint the regex match to a certain position. ```^``` this anchor is used to match the position before the first character in the string whereas the ```$``` anchor is used to match right after the last character within the string. 

## Quantifiers
Quantifiers set the limit of the minimum and maximum number of characters within the string, it works by specifying how many characters, groups or character classes must be present for a match to be found. They are known as being greedy characters because they want to match as many characters as possible. Quantifiers such as ```*```, ```+```, ```?```, ```{}``` are found within regular expressions. The ```*``` quantifier matches the pattern zero or more times. The ```+``` quantifier matches the pattern one or more times. The ```?``` quantifier matches the pattern zero or one time. The ```{}``` quantifier sets limits in three different ways, ```{n}``` matches the pattern EXACTLY n amount of times, ```{n,}``` matches the pattern at LEAST n amount of times and lastly, ```{n, x}``` matches the pattern from a minimum n amount of times to a maximum x amount of times. The Hex Value regular expression has 6 and 3 color values, this indicates that the length of the component preceding these quantifiers should be 6 and 3 characters

## OR Operator
The OR operator helps to indicate that the values could be any of the components that is being separated with ```|```, in the HEX value regex two components are separated by the OR operator meaning that the HEX value could be 6 or 3 characters.

## Character Classes
A character class is used to define a set of characters that occurs in an input string to fulfill a match meaning it indicates what type of characters to expect within the regex. Common character classes include ```[]```, ```.```, ```\d```,```\w```,```\s```. The ```[]``` class indicates a range of characters that we want to match. The ```.``` class matches any character except the newline character ```\n```. The ```\d``` class matches any arabic numeral character this is ~ to the ```[]```. The ```\s``` class matches a single whitespace character such as tabs and line breaks. In the HEX value regex it contains two classes such as ```[a-f0-9]``` and ```[a-f0-9]```, these character classes are searching for letters ```a-f``` and numbers between ```0-9```.

## Flags
Flags are found at the end of the regex and they work to define any additional functionality or limits, a regex is wrapped around slashes however flags are found outside of the slashes. You'll see flags such as ```g```, ```i```, ```m```. The ```g``` is a global search to test all possible matches in a string. The ```i``` is a case insensitive search to be ignored when attempting a match within a string. The ```m``` is a multiline search that has a string that should be in multiple lines. In this case flags are not within the HEX value regex. 

## Grouping and Capturing
Grouping constructs use ```()``` to group sections within a regex. Regular expressions can have multiple parts to a string fulfilling a specific requirement. These sections are broken down by using grouping constructs. In this case the HEX value regex doesn't have more than one section to group. 

## Bracket Expressions
Bracket expressions indicates a range of characters that we want every character to match; these brackets are known as a positive character group due to it being characters we want to match.

## Greedy and Lazy Match
A greedy match like quantifiers, works by trying to match every possible elements however a lazy match does the opposite by trying to match an element a little amount of times possible. 

## Author
Kayla Rosario - Full Stack Web Developing student -
[Github](https://github.com/krosario314)