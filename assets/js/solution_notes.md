- start with review of main HTML file
- talk about running the application (directly in the browser)

## Assignment notes

Assignment 1:
The canvas is rather small. Increase it by adjusting the canvas size value in settings.js.
_increase to 20x20_

Assignment 2:
The snake moves once every 30 frames. Now that the canvas size has been increased this is rather slow.
Make it move more frequently by reducing the frame counter limit near the top of game.js.
_7 is a good limit_

Assignment 3:
The input controls only work in two directions. Implement controls for the other two directions.
Look at how controls for the other two directions were implemented near the bottom of game.js.

Assignment 4:
Right now the snake wraps around when it reaches the edge of the game screen. In some versions of the game hitting the edge ends the game.
Make the necessary changes to the checkEdgeCollision() function so that the game resets when the snake hits any of the edges of the screen.

Assignment 5:
The score system doesn't work. Give the player points whenever an apple is eaten by increasing the value of the score variable.

_update update score_
_good option for question_
_also update in reset game_

Assignment +:
Give the snake a random color whenever an apple is eaten. Make sure it's not too dark or you won't be able to see the snake.

_const hueColor = Math.random() \* 360;_
_snake.color = `hsl(${hueColor}, 100%, 70%)`;_

https://www.w3schools.com/css/css_colors_hsl.asp

Assignment +:
Increase the snake's speed for every x amount of apples that are eaten.

_In eat Apple: `frameCounterLimit = frameCounterLimit * 0.9;`_
_Also set initial value constant and reset in reset game._

Assignment +:
Add a golden apple to the game. It has a 10% chance to appear instead of the regular apple every time an apple is eaten.
It grants more scorepoints than the regular apple.
