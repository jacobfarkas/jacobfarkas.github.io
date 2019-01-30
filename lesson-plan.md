## Lesson Plan - Creating Dice using p5.js

### Overview

In this lesson, students learn how to host a p5.js project using the **Glitch** platform. Students also learn how how to sketch a pair of dice using the `draw` *function* in p5.js. There is also a brief discussion how to best determine the **x** and **y** coordinates on the canvas by adding a line of code.

## Lesson Sequence
		
#### Setup a Glitch account
---

Have a student lead a live-coding session and do the following:

- Create a [glitch](https://glitch.com) account

- Create a new project in Glitch

#### Prepare the Glitch project to host a p5.js project
---
- In the Glitch project, create a new blank file, titled `sketch.js`
- Create a new `index.html` file, which will be used to point to the newly created `sketch.js`file.

**Add the p5.js links via CDN**
Edit the `index.html` to include the following in the `<head>`:  
``` 
<!-- import the webpage's p5js pages -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/0.7.1/p5.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/0.7.1/addons/p5.dom.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/0.7.1/addons/p5.sound.min.js"></script>
 ```
- Add a link to the newly created `sketch.js` file right before the closing tag of the `</body>`
in the `index.html`.
```
<!-- p5js -->
<script src="sketch.js"></script>
```
The full code for the `index.html` can be seen [here](https://github.com/lrei-coding/p5js_18-19/blob/master/dice/index.html).

- Go through a step-by-step breakdown of the code for [this project](https://quiet-timer.glitch.me/):
    - Creating the Canvas
    - Using the `draw` *function* to create Dice
    - Draw ellipses in the proper place for the dice value
    - **(TIP)** Have **text** display on top, with the X and Y coordinate values, refresh live with mouse movements, to aid with the drawing process. This can be done by adding the following in the beginning of the draw function.  
```text('X: ' + Math.round(mouseX) + '     ' + ' Y: ' + Math.round(mouseY), 10, 14);```

This reviews many of the core concepts that were addressed in the [first week's class](https://github.com/lrei-coding/p5js_18-19/blob/master/class-notes/2019_01_09.md), in the [peblio hour of code](https://demo.peblio.co/pebl/AXcwQlcDZ).

Students are expected to make all six versions of the dice for both the top and bottom dice and leave them all commented out, except for the ones they are displaying at the time.

## Dice Project

This is a multi-week project and includes the following milestones:
1) Create a 2D visualization of the dice. [Assignment can be found here](https://github.com/lrei-coding/p5js_18-19/blob/master/dice/dice-assignment_01.md).
2) Add some buttons with values 1-6 that a user can select and it will draw a corresponding die with that value
3) Have an animation that can roll the dice and have them randomly selected. 
