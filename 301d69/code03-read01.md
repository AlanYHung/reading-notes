# Code 301
## Reading 01
##### (All My Notes are attributed/sourced from the Resources directly preceding them.)


[Responsive Web Design](https://learn.shayhowe.com/advanced-html-css/responsive-web-design/)
* Responsive Web Design is about building web sites suitable to all the different kinds of devices and screen sizes.
* Responsive vs Adaptive vs Mobile
  - Responsive - reacts quickly and positively to any change
  - Adaptive - easily modified for new purpose or situation
  - Mobile - means to build solely for mobile devices
* 3 Main Components
  - Flexible Layouts - practice of building websites using flexible grids capable of dynamic resizing
    1. vw - Veiwports Width
    1. vmin - Minimum Viewport Height and Width
    1. vh - Viewports Height
    1. vmax - Maximum Viewport Height and Width
  - Media Queries - provide the ability to specify different styles for individual browser and device circumstances
    1. uses logical operators and, not, and only to allow for test of device capabilities
    1. Media Features identify what attributes or properties will be targeted within the media query expression
      * Orientation Media Feature - determines if devices views in Landscape or Portrait
      * Aspect Ratio Media Feature - keeps element width to height ratio proportional no matter screen size
      * Pixel Ratio Media Feature - used for high definition devices
      * Resolution Media Feature - specifies resolution of output device in pixel density
    1. Media Queries do not work with Internet Explorer 8 and below or any other legacy browsers.
  - Flexible Media - changing the size of media such as images and videos to fit a device's viewport
    * Does not work well for embedded media such as in iframes, but there is a workaround by positioning the embedded element absolutely in parent element.  The parent element then  has to be flexibly scalable to viewport.


[All About Floats](https://css-tricks.com/all-about-floats/)
* Float is a CSS Positioning Property
* Float can be used to allow text to wrap around image elements
* Float can be used to create entire web layouts
* Clear - when set on an element, it will move the element below the floated elements
  * Both - most commonly used attribute of clear, which clears floats of both directions left or right.
  * Left - clears Float: Left
  * Right - clears Float: Right
  * None - Default Value, but unnecessary unless removing another clear
* Can cause parent element to think it doesn't contain anything and collapse height of the parent element
* Methods to Clear Float
  1. The Empty Div Method - \<div style="clear: both;"\>\</div\> sometimes, more rare, may see \<br\> or equivalent
  1. The Overflow Method - relies on setting overflow css property to the parent element, which clears float for any succeeding elements
  1. The Easy Clearing Method - uses selector (:after) to clear floats

    ```
    .clearfix:after { 
      content: "."; 
      visibility: hidden; 
      display: block; 
      height: 0; 
      clear: both;
    }
    ```

* Problems with Floats
  - Pushdown - an element inside the floated item being wider than the floated item
  - Double Margin Bug - Applying a margin in the same direction as a float doubles the margin
  - 3px Jog - text next to a floated element is pushed away by 3px
  - Bottom Margin Bug - floated parent has floated children inside it, bottom margin of children is ignored by parent


[Don’t Overthink It Grids](https://css-tricks.com/dont-overthink-it-grids/)
* Vast majority of websites use a grid
* Context - width: auto makes content inside a parent as wide as the parent
* Columns - Float 2 elements then split 100% width between 2 elements
* Clearing Context - Fixing Floated Parent height with floated Children

  ```
  .grid:after {
    content: "";
    display: table;
    clear: both;
  }
  ```

* Gutters - Set gutters to fixed pixel sizes to keep design more stable

  ```
  *, *:after, *:before {
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
  }
  ```

* Outer Gutters - Set Gutters for entire page


[CSS Floats Explained By Riding An Escalator](https://www.freecodecamp.org/news/css-floats-explained-by-riding-an-escalator-57fa55232333/)
* Floats have 2 different Flows Left and Right
* You can reset Floats using clear


[Scalable and Modular Architecture for CSS](http://smacss.com/)
> SMACSS (pronounced “smacks”) is more style guide than rigid framework. There is no library within here for you to download or install. There is no git repository for you to clone. SMACSS is a way to examine your design process and as a way to fit those rigid frameworks into a flexible thought process. It is an attempt to document a consistent approach to site development when using CSS. And really, who isn’t building a site with CSS these days?!
  * [SMACSS Reading](smacss-2012-08-21.pdf)




[<-- Back](../README.md)
