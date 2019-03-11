# HTML5

So glad you could make it! So you say you like `HTML`? Or are you just bored? Well, either way we have got you covered!

First thing first is you need to understand that most of the time a simple Google search would solve your problems. In some, it may not.

Let's say we want to have a Flappy Bird example of the game. Let's start creating it.

## Canvas

The HTML <canvas> element is displayed as a rectangular object on a web page.
The <canvas> element is perfect for making games in HTML.
The <canvas> element offers all the functionality you need for making games.
Use JavaScript to draw, write, insert images, and more, onto the <canvas>.
The <canvas> element has a built-in object, called the getContext("2d") object, with methods and properties for drawing.
To make a game, start by creating a gaming area, and make it ready for drawing:
``` js
function startGame() {
  myGameArea.start();
}

var myGameArea = {
  canvas : document.createElement("canvas"),
  start : function() {
    this.canvas.width = 480;
    this.canvas.height = 270;
    this.context = this.canvas.getContext("2d");
    document.body.insertBefore(this.canvas, document.body.childNodes[0]);
  }
}
```
The object myGameArea will have more properties and methods later in this tutorial.

The function startGame() invokes the method start() of the myGameArea object.

The start() method creates a <canvas> element and inserts it as the first childnode of the <body> element.

## Game Components

Make a component constructor, which lets you add components onto the gamearea.

The object constructor is called component, and we make our first component, called myGamePiece:

``` js
var myGamePiece;

function startGame() {
  myGameArea.start();
  myGamePiece = new component(30, 30, "red", 10, 120);
}

function component(width, height, color, x, y) {
  this.width = width;
  this.height = height;
  this.x = x;
  this.y = y;
  ctx = myGameArea.context;
  ctx.fillStyle = color;
  ctx.fillRect(this.x, this.y, this.width, this.height);
}
```
## Frames

To make the game ready for action, we will update the display 50 times per second, which is much like frames in a movie.

First, create a new function called updateGameArea().

In the myGameArea object, add an interval which will run the updateGameArea() function every 20th millisecond (50 times per second). Also add a function called clear(), that clears the entire canvas.

In the component constructor, add a function called update(), to handle the drawing of the component.

The updateGameArea() function calls the clear() and the update() method.

The result is that the component is drawn and cleared 50 times per second:
``` js
var myGameArea = {
  canvas : document.createElement("canvas"),
  start : function() {
    this.canvas.width = 480;
    this.canvas.height = 270;
    this.context = this.canvas.getContext("2d");
    document.body.insertBefore(this.canvas, document.body.childNodes[0]);
    this.interval = setInterval(updateGameArea, 20);
  },
  clear : function() {
    this.context.clearRect(0, 0, this.canvas.width, this.canvas.height);
  }
}

function component(width, height, color, x, y) {
  this.width = width;
  this.height = height;
  this.x = x;
  this.y = y;
  this.update = function(){
    ctx = myGameArea.context;
    ctx.fillStyle = color;
    ctx.fillRect(this.x, this.y, this.width, this.height);
  }
}

function updateGameArea() {
  myGameArea.clear();
  myGamePiece.update();
}
```

## Make it move

To prove that the red square is being drawn 50 times per second, we will change the x position (horizontal) by one pixel every time we update the game area:

``` js
function updateGameArea() {
  myGameArea.clear();
  myGamePiece.x += 1;
  myGamePiece.update();
}
```
### Why Clear the Game area?

It might seem unnecessary to clear the game area at every update. However, if we leave out the clear() method, all movements of the component will leave a trail of where it was positioned in the last frame:

``` js
function updateGameArea() {
  // myGameArea.clear();
  myGamePiece.x += 1;
  myGamePiece.update();
}
```

## Homework

1) Try to understand what happened in the following tutorial code and try to add the following:
- Game Controllers
- Game Obstacles
- Game Score
- Game images
- Game Sound

2) Look at `game.html` and see what needs to be changed and how we can improve it? (Example, how would you add a score to the game? Timer? Enemies?)

3) Let me know if you would like to know how to create the [following](http://www.lostdecadegames.com/demos/simple_canvas_game/) game? If so, we will finish with this one in the
next lesson and start with this one.

4) The final project would be to create a Zombie Apocalypse Survival Game using GPS service
