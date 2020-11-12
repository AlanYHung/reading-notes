# Code 201
## Reading 14a

[CSS Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)
* New CSS3 Element for positioning and altering elements
* Has 2 different settings
  1. two-dimensional
  1. three-dimensional
* This property still does not have good browser support as of yet.

```
=========== Sample Code ===========

div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
```


[Transitions & Animations](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)
* CSS3 provides the ability to write behaviors for transitions and animations
* Transitions can alter the appearance or behavior of element based on user actions
  1. hover over
  1. focus on
  1. active
  1. targeted
* There are [8 simple but useful Transitions](http://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users) that will make your page look better
  1. Fade In
  1. Change Color
  1. Grow & Shrink
  1. Rotate Elements
  1. Square to Circle
  1. 3D Shadow
  1. Swing
  1. Inset Border
* Animations allow the appearance or behavior of element to be altered in multiple keyframes
* Here is sample code to show Animations used in [6 different ways on Buttons](https://codepen.io/retyui/pen/ByoaXV).
* Here is sample code to show Animations using [Keyframes](https://codepen.io/akshaychauhan/pen/oAfae)

```
=========== Sample Transition Code ===========

.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}
```

```
=========== Sample Animation Code ===========

@keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}
```


[404](https://codepen.io/kieranfivestars/pen/MYdQxX)
* This code shows how you can combine Transform and Animation together to uniquely display the numbers 404

[Bounce Animation](https://codepen.io/dp_lewis/pen/gCfBv)
* Uses Transform and Animations to create a bouncing object



[<-- Back](../README.md)
