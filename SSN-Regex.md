# Regex Tutorial: Social Security Numbers

In this tutorial, I will be breaking down and summarizing the usage and purpose of “Regex” or regular expressions.  I will demonstrate how the principal properties of regular expressions are applied to social Security Numbers.  

## Summary

Before we begin, I should explain what regex is. In a nutshell, it is special strings representing a pattern that matches or locates in a body of text.   Used by all programming languages, it has a wide variety of uses. 
Our example works with SSNs which is a sequence of 9 digits formatted as 3 numbers followed by a dash then 2 numbers followed by a dash then 4 numbers followed by a dash. 
Here is what the Social Security Number validation looks like: 

```
^\d{3}-\d{2}-\d{4}$
```

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)



## Regex Components

### Anchors

To keep it simple, anchors are boundaries at the beginning of the string `^`, and the end of the string `$`.  The Boundaries examines the position between characters.
In our SSN example, you can see the symbols signaling the beginning and end of our validation regex.  Our expression will search for strings that begin with `{n}` and end with `{n}`.

### Quantifiers
Quantifiers tell us how many times a character should be present for a match to be found. 
Basic quantifiers: 

```
*	0 or more characters  
+ 	1 or more characters 
? 	0 or 1 
{} 	Exact match 
```

In our SSN example, we were looking for a format that looks exactly like this:

```
000-00-0000
```

Which would be translated in our Validation to look like this: 

```
^\d{3}-\d{2}-\d{4}$
```

### Character Classes

To simplify it, character classes are used to distinguish between numbers and letters. Since SSNs are a series of 9 digits only, we used the character class `\d`. 
Here are some other characters used: 

```
\d 	Numbers 0 -9 
\w 	Letters A-Z , a-z , 0-9) 
\s 	White space 
•	Any character
```

## Author

Mohamed is a Full-Stack Developer. To browse my projects or find my contact information, visit [GitHub](https://github.com/mo9399) or [linkedIn](https://www.linkedin.com/in/mohamed-abdullahi-944b2922b/) page!