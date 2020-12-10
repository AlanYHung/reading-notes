# Code 301
## Reading 09
##### (All My Notes are attributed/sourced from the Resources directly preceding them.)


### Concepts of Functional Programming in Javascript 
#### Author: TK
[Article Source](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)
* System Complexity is anything that makes the code hard to understand or modify
* Functional Programming is a style of building the structure of computer programs to work like mathematical functions where it evaluates and returns data
* Pure Functions are Functions that return the same result everytime if the arguments do not change and they do not cause any noticeable side effects.
* Examples of Impure Functions:
  * A Function getting data from a file is not considered a pure function because the contents of the files can change
  * Any Random Number Generator is not considered a pure function
  * Modifying a Global Variable is an example of noticeable Side Effects
* Benefits of Pure Functions is that the code is easier to test
* Immutable data is data that cannot be changed after creation
* Referentially Transparent - a function that returns the same result when given the same input
* Functions as first-class entities:
  * Can be referred to from constants and variables
  * Can be passes as a parameter to other functions
  * Can be returned as a result from other Functions
* High Order Functions:
  * Takes one or more functions as arguments
  * Returns a function as the result
* The Filter Function lets you use conditional statements to target the data you want to return/keep
* The Map Function lets you transform the values of your table and builds a new collections of values for the result
* The Reduce function takes a function and a collection of values and returns a value created by combining the parameters



### Refactoring JavaScript for Performance and Readability (with Examples!)
#### Author: Andrew Healey
[Article Source](https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec)
* Strategies for implementing methods to make code easier to read
  * Return early from functions
  * Cache variables so functions can be read like sentences
  * Check for Web APIs




[<-- Back](../README.md)
