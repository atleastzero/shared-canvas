# shared-canvas
 
Shared Canvas is a project where you are responsible for a a single square in a grid. Draw whatever you like in your grid square!

## Getting Started

Find your name on the grid. You're responsible for making sure your drawing ends up in that location. 

Each grid square is 113px by 113px. 

The canvas is 6 by 5 grid squares and 678px by 565px. 

- Width 6 squares (113px * 6) 678px
- Height 5 squares (113px * 5) 565px

For example: Mitchell has been assign to square 4, 3. All of the drawing they do must fall within a square starting at x of 452 and y of 339 and ending at x of 565 and y of 452. 

- left 4 * 113 = 452
- top 3 * 113 = 339
- right 4 * 113 + 113 = 565
- bottom 3 * 113 + 113 = 452

Here's a picture illustrating where their drawing should end up. 

![grid map overlay](notes/shared-canvas-overlay.png)

To draw you should create a JS with your name. In this file import `ctx` and `size`.

```JS
import ctx, { size } from './main.js'

const x = 4 * size
const y = 3 * size
```

`ctx` is your drawing context. Use to call any of the drawing methods. 

`size` is the a constant that defines the size of each square (113.)

The constants x and y that have define above locate the upper left corner of the box that I will draw in. 

Take a look at [mitchell.js](mitchell.js) to get ideas on how to draw shapes. 

Find your name in the image below and adjust your drawing so that is draws within the correct location. 

![grid map](notes/shared-canvas.png)

