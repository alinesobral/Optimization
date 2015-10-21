To run this aplication, go to http://alinesobral.github.io/Project4
This application is a simple portfolio. You can access some of Cameron's featured work on the links provided.
On the Cam's Pizzeria website you can build your own pizza and choose its size.

=============================================================================================================
The biggest optimizations made by the student are outlined below:


1) The size of the profile picture and the pizzeria picture were reduced.
2) The html was minified.
3) The print and screen media queries on the style.css file were made into two separate files (print.css and media.css) and called on the head of the html file.
4) The javascript files on lines 22 and 23 of the html file are now async.
5) On views > css > style.css:
	a) Added vendor prefixes on .mover
6) On views > js > main.js:
	a) On the changePizzaSizes function (line 453) the size of the pizzas were kept in percentage values to avoid a forced synchronous layout due to changing values between pixels and percents.
	b) Changed some .querySelectorAll to .getElementsByClassName/ .getElementById in order to increase perfomance.
	c) On lines 517-519 the number of pizzas on the background of the page was calculated according to the size of the screen.
	d) On the updatePositions function: some variables were declared outside the for loop, so they don't have to be declared (var) in each loop.
	e) On line 470: declared randomPizzas.length; outside the for loop.
	f) On line 488: declared the pizzaDiv variable outside the loop so there's only one DOM call.
	g) On line 554: declared elem outside the for loop.
7) The font on index.html is now loaded using Javascript.
8) The contents of style.css were inlined on the index.html file.