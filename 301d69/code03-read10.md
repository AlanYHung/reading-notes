# Code 301
## Reading 10
##### (All My Notes are attributed/sourced from the Resources directly preceding them.)


### Call Stack
#### Author: Mozilla and Individual Contributors
[Article Source](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)
> A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions
  * > When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
  * > Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
  * > When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
  * > If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.
###### (NOTE: All the above notes comes directly from the Article word for word)



### The JavaScript Call Stack - What It Is and Why It's Necessary
#### Author: Charles Freeborn
[Article Source](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)
* Understanding the call stack helps give clarity to the function hierarchy and function execution order.
* The call stack is mostly used for function calls
  * Since JavaScript is single threaded, functions execute in synchronous order
  * A stack works as a type of list following the LIFO (Last In First Out) execution sequence.
* Asynchronous JavaScript uses a callback function, an event loop, and a task queue.
* A stack overflow happens with a recursive function hits an infinite loop




### JavaScript error messages && debugging
#### Author: Diogo Spínola
[Article Source](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)
* A bug is unexpected behavior of code that does not work as intended
* Ways to identify bugs your code:
  * Error Messages
    1. Reference Errors - trying to use variables that have yet to be declared
    1. Syntax Errors - missing, misplaced, misspelled, or extra characters in your line of code
    1. Range Errors - trying to manipulate variables outside of their scope
    1. Type Errors - trying to change the type of a variable, such as putting a string into a numeric variable
  * console.log
  * breakpoints
  * Tools to try to avoid errors:
    1. quokka
    1. eslint
    1. TypeScript
* Handling Errors
  * Try and Catch are methods designed to try to handle errors


  ### Additional SQL Resources
  * [JavaScript errors reference on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)




[<-- Back](../README.md)
