# Regex-Tutorial

RegEx Tutorial
RegEx, short for 'regular expression', is a pattern of characters used to validate combinations of those characters. The following tutorial takes a commonly used regex pattern, used to validate an email address, and amalgamate its basic concepts. 


### RegEx Example:
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

The above code is used to validate whether an input is an email address or not. The tutorial will break down its components to further explain its functionality. 


### Regex Components

### Anchors:
Anchors are used to specify positions of specific characters. 

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

For example, the carat '^' is used to define the beginning of the string, whereas the dollar sign '$' is used to identify the end of the string. 

### Quantifiers

A quantifier is what's known as a repetition operator. Quantifiers communicate with the system to inform it to match the token a predefined number of times.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

For example, the star '*' will match zero of the token, and the question mark '?' makes the token optional. 


### Character Classes
A character class matches one of the characters--the order does not matter. 

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

I've provided a couple of examples of character classes not seen in the above example. 

The unicode 'u' allows for extended unicode escames in the form
Digit '/d' will match any number
Word '/w' will match any word 

### Grouping and Capturing
Groups combines multiple tokens and operates on them together

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

The example above uses three capturing groups: ([a-z0-9_\.-]+), ([\da-z\.-]+), and ([a-z\.]

These permit a substring to be verified before '@', before '\.', and the domain of the email address, respectively.

### Greedy and Lazy Match
Quantifers are organized into being either greedy or lazy. The affectionately known greedy quantifier will attempt to match as many characters as possible whilst traversing backwards through the string, whereas a lazy quantifier matches as few as possible. The default quantifier is greedy unless it is affected by another quantifier. 


### About the Author
Gus is a recent college graduate trying to become a software developer. You can find his profile at https://github.com/August-Lascola
