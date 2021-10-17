# Email-Gist

Regex is defined as a regular expression. In other words it is a character sequence that can be used in search pattern, to find or replace characters in a given text or to validate input.

It is widely used in extracting information from any text or paragraphs. Regex is also used in code, search algorithms and validation in diffrent types of programming languages


# Summary

We will be discussing on Matching an Email code snippet – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

Breaking this code snippet in 3 small pieces may help easily understand components and their importance in specific location.
It is as below -   

First : /^([a-z0-9_\.-]+)    represents email or username

Second : @([\da-z\.-]+)      represents email service provider

Third : \.([a-z\.]{2,6})$/   represents domain ( e.g.  .com or .gov)


# Table of Contents

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

# Regex Components

Regex contains different components such as Anchors (^ $), Quantifiers ( * + ? {}), OR operator ( | or [ ]), character classes ( \d, \w, \s . ), and Flags ( g, m, i ).

We will try to explain each below on it's role in Email code snippet – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ 


# Anchors

In code snippet above, the ^ and $ are considered as anchors. The ^ indicates the starting point of the string while $ indicates the end point of the string. All components except / are used in between Anchors. 


# Quantifiers

This Email code snippet includes +  and { } quantifiers. 

The + sign in first and second piece repeats the preceding regex one or more times. In ([a-z0-9_\.-]+) it matches one or more letter, digit, underscore, fullstop, and hyphens.

The {2, 6} in third piece represents minimum and maximum number of characters match allowed after fullstop (.) respectively 

# Character Classes

The \d  in  @([\da-z\.-]+)  represents character class. It matches only a single character that should be a digit from 0 to 9. No more than one character digit will be allowed in this case.


# Grouping and Capturing

Grouping and capturing is presented by (). In the code snippet above, we have 3 capturing group as they are broken in 3 small pieces. These capturing group represents username, service provider and domain respectively. 


# Bracket Expressions

Bracket Expression is presented by [ ].  
In [a-z0-9_\.-], it matches letter a to z, digit 0 to 9, underscore, hyphen, and fullstop.
In [\da-z\.-], it matches one single digit, letter a to z, hyphen, and fullstop. 
In [a-z\.], it matches letter a to z, and fullstop.


# Greedy and Lazy Match

 The + and { } are greedy match used in our code snippet. 
 The + expands the match as far as it can through the provided text. 
 {2,6} expands matching characters that are 2 to 6 characters in length.


# Boundaries

Boundaries are represented by \b and \B. It is used in whole words only search. In our code snippet boundaries are not used.


# Author

Umair Ali <br>
Please view my profile at: https://github.com/umairali-bit
