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

