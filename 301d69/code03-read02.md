# Code 301
## Reading 02
##### (All My Notes are attributed/sourced from the Resources directly preceding them.)


### JavaScript & JQuery
#### JQuery (pp. 293-335)
* JQuery is a JavaScript file you include in your web pages that lets you find and use elements through CSS-style selectors which you can manipulate with JQuery methods.
* Offers a simple way to quickly and consistently achieve variety of common JavaScript tasks across all major browsers without needing fallback code.
* Why use JQuery?
  1. Makes coding simpler
  1. Simple Selectors
  1. Common tasks in less code
  1. Cross-Browser Compatibility
* List of jQuery selectors and methods (pp. 302-305)
* A Matched Set / jQuery Selection - when you select one or more elements, a JQuery object is returned.
* Some jQuery methods both retrieve information from, and update the contents of, elements.  Does not apply to all elements.
* jQuery Objects store references to elements
* Method .ready() checks that the page is loaded and ready to work with your code.
* Getting Element Content (p. 314)
  1. .html() - retrieves only the html inside the first element
  1. .text() - retrieves the text from the element.
* Updating Elements (p. 316)
  1. .html()
  1. .text()
  1. .replaceWith() - replaces every element in a matches set with new content
  1. .remove() - removes all elements in a matched set
* Inserting Elements (p. 318)
  1. .before()
  1. .after()
  1. .prepend()
  1. .append()
* Getting and Setting Attribute Values (p. 320)
  1. .attr()
  1. .removeAttr()
  1. .addClass()
  1. .removeClass()
* .css() lets you retrieve and set values of CSS properties
* .each() allows you to recreate the functionality of a loop on the selection of elements
* .on() is used to handle all events
  - Has 2 methods optional methods that let you filter the initial jQuery selection to a subset element and pass extra information to event handler using object literal notation.
* jQuery has effect methods to help with transition and movements of elements (p. 332)
  1. Basic Effects
    * .show()
    * .hide()
    * .toggle()
  1. Fading Effects
    * .fadeIn()
    * .fadeOut()
    * .fadeTo()
    * .fadeToggle()
  1. Sliding Effects
    * .slideUp()
    * .slideDown()
    * .slideToggle()
  1. Custom Effects
    * .delay()
    * .stop()
    * .animate() - allows you to make custom effects and animations
* 
#### JQuery (pp. 354-357)
* You can load jquery from a CDN (Content Delivery Network)
* Where to place your Scripts
  1. Head - not ideal as it makes your pages slower to load
  1. Body - not ideal will make whatever is after slower to load
  1. before \</body\> ideal location as the entire page will have loaded already before loading your script files


[6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)
1. Greater Efficiency
1. Engaged Collaboration
1. Learning from fellow students
1. Social skills
1. Job interview readiness
1. Work environment readiness



[<-- Back](../README.md)
