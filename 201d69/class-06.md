# Code 201
## Reading 06
##### (All My Notes are attributed/sourced from the Resources directly preceding them.)

### JavaScript & JQuery
#### Object Literals (pp. 100-105)
* Objects are a set of variables and functions that model something you would recognize in the real world.
* Variables within Objects become known as Properties
* Functions within Objects become known as Methods
* Literal Notation is the easiest and most popular way to create objects
    * var [Variable Name] = {
        [Variable Name]: <Value>,
        [Function Name]: function() {
            [Code goes here];
        }
    }
* Dot Notation is used to access the values within an Object

#### Document Object Model (pp. 183-242)
* The browser represents the page using a DOM (Document Object Model) tree.
* Four types of Nodes in DOM Tree:
    1. Document Nodes
    1. Element Nodes 
        * Can be Selected by:
            1. id or class attributes
            1. tag name
            1. CSS selector syntax
        * Properties used to access and change content
            1. textContent
            1. innerHTML
            1. DOM Manipulation Techniques
                * Refers to using a set of methods and properties to access, create, and update elements
        * Can contain multiple text nodes and direct child elements
    1. Attribute Nodes
    1. Text Nodes
* When a DOM query returns more than one Node, it is returning what is called a Node List
* Browsers offer tools that enable you to see DOM Tree


[<-- Back](../README.md)
