# Code 201
## Reading 12

[Article on Chart.js](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)
* You can create animated charts with Chart.js
* Chart.js is a javascript plugin
* [Chart.js Download](https://github.com/nnnick/Chart.js)
* This article has sample code for many different types of charts (i.e. Line, Pie, and Bar)
* [Chart.js Documentation](https://www.chartjs.org/docs/latest/)

```
==========================================================================================================================
Sample Line Graph Code  |  https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/
==========================================================================================================================
<canvas id="buyers" width="600" height="400"></canvas>

<script>
    var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
</script>

var buyerData = {
	labels : ["January","February","March","April","May","June"],
	datasets : [
		{
			fillColor : "rgba(172,194,132,0.4)",
			strokeColor : "#ACC26D",
			pointColor : "#fff",
			pointStrokeColor : "#9DB86D",
			data : [203,156,99,251,305,247]
		}
	]
}
```

#### Canvas API
* [Canvas API - Basic Usage](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)
  * \<canvas\> Element
  * Type of image element with the only difference being there is no src and alt attributes
  * Canvas Element requires a closing tag
  * Lots of sample code on this site
* [Drawing Shapes with Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)
  * Canvas Element has a grid or coordinate space you can use to draw shapes
  * Drawing Rectangles has 3 functions
    1. fillRect(x, y, width, height) - Draws Solid Rectangle
    1. strokeRect(x, y, width, height) - Draws Rectangle outline
    1. clearRect(x, y, width, height) - Makes Rectangle Transparent
  * You can draw paths using multiple points and connecting them
    1. beginPath() - Creates a new path
    1. closePath() - Adds a straight line between points of Path
    1. stroke() - Draws the shape outline
    1. fill() - fills in the path's content area
  * There are several other functions and shapes on this to be used as a reference if ever needed
* [Applying styles and colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)
  * After Drawing shapes you can fill them with colors
  * fillStyle = color - color shape
  * strokeStyle = color - outline shape with color
  * You can also set the transparency of a shape by setting the transpareny value of a shape using something like rgba
  * You can add Line caps to your path lines, like rounding off the tips using the lineCap property
  * Other things you can do are adjust Gradient, Shadows, and patterns
* [Drawing Text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)
  * 2 methods to render text on a canvas
    1. fillText(text, x, y [, maxWidth])
    1. strokeText(text, x, y [, maxWidth])
  * Text can be styled using properties
    1. font = value
    1. textAlign = value
    1. textBaseline = value
    1. direction = value


[<-- Back](../README.md)
