## Lesson Plan - x-block p5.js
**1-16-2019**
Creating Dice in p5js

Student led a live-coding session and did the following:

- Created a [glitch](https://glitch.com) account

- Created a new project in Glitch, and created a new blank file, `sketch.js`
- **Added p5js links via CDN**
  
Edited the `index.html` to include the following in the `<head>`:  
``` 
<!-- import the webpage's p5js pages -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/0.7.1/p5.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/0.7.1/addons/p5.dom.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/0.7.1/addons/p5.sound.min.js"></script>
 ```
- Added a link to the newly created `sketch.js` file right before the closing tag of the `</body>`
in the `index.html`.
```
<!-- p5js -->
<script src="sketch.js"></script>
```
The full code for the `index.html` can be seen [here](https://github.com/lrei-coding/p5js_18-19/blob/master/dice/index.html).

- Went through a step-by-step account of the code for [this project](https://quiet-timer.glitch.me/):
    - Create Canvas
    - Use the draw function to create Dice
    - Draw ellipses in the proper place for the dice value
    - (TIP) Have **text** display on top, with the X and Y coordinate values, refresh live with mouse movements, to aid with the drawing process. This can be done by adding the following in the beginning of the draw function.  
```text('X: ' + Math.round(mouseX) + '     ' + ' Y: ' + Math.round(mouseY), 10, 14);```

This reviews many of the core concepts that were addressed in the [first week's class](https://github.com/lrei-coding/p5js_18-19/blob/master/class-notes/2019_01_09.md), in the [peblio hour of code](https://demo.peblio.co/pebl/AXcwQlcDZ).

Students are expected to make all six versions of the dice for both the top and bottom dice and leave them all commented out, except for the ones they are displaying at the time.

## Dice Project

This is a multi-week project and includes the following milestones:
1) Create a 2D visualization of the dice. [Assignment can be found here](https://github.com/lrei-coding/p5js_18-19/blob/master/dice/dice-assignment_01.md).
2) Add some buttons with values 1-6 that a user can select and it will draw a corresponding die with that value
3) Have an animation that can roll the dice and have them randomly selected. 
