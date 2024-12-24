[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/6l4sY1d2)
# Assignment 2: Play with a 2x2 Rubik Cube
by 

**NAME**: MUHAMMAD NORAZLAN BIN A SAMAT@SAMAD

**Matric ID**: 2116455

## Objective

1. Accept the assignment and make sure you have a copy of the code.
2. The code provide a partially working code.
3. Add the necessary faces of the rubik cube in the code.
4. Modify the logic for rotating the 2x2 cube.
5. Add buttons below the cube to create action buttons.
6. Create a simple 2x2 rubik cube application that allows the user to rotate the faces of a rubik cube. The code given doesn't work. You may have to read the code and complete some functions and add buttons.
7. Make sure to only submit your /lib folder and modify the readme to describe what was done. You must also include your name and matric ID in this readme file.

## Requirements:

Tips:
Make sure to look at https://docs.flutter.dev/cookbook/lists/grid-lists to get a hang of the flutter grid layout which is being used in the code.

## What was Done

### Step 1: A clear view of the problem and what to do
1. The code given has already labeled the color of the whole rubik's cube being front with red, left with blue, right with green, back with yellow, top with orange, and bottom with white.

2.The objective is to make the rubik's cube to rotate and play like a rubik's cube with a constraint of it being on one way only (Dominantly rotate to the left, and rotating downwards)

3. A rubik's cube can be played via rotating the top row, and bottom row (to go to the left) or rotating the left column or right column (to go downwards)

4. The rubik's cube cell of every face will be labeled under an array in a list, and the rotation would happen by moving the array around.

5. Therefore, I identified that first, each cell of all face of the rubik's cube must be properly labeled in a list first.

6. Add 4 type of button, rotate top row, rotate bottom row (both moving to the left), rotate left column, rotate right column (both moving downwards).

7. To ease testing, I'll also add a reset button to make sure I can reset and properly see how the rubik's cube movement and not just get lost in the colors when i play around with it.

### Step 2: reset function
1. To ease making the reset button, i set the faces to initialFaces and relist faces as an empty string

2. made a function called void resetFaces() whereby faces will be filled with the initialFaces mapping and set it under CubeState() to initialize the reset faces function

3. The button will be made later

### Step 3: rotateTop() function

1. I didn't change anything except for the rotation of the top view, as i need to start with [2] [0] [3] [1] and not [2] [3] [0] [1]. Im not sure why, but i think it has something to do with logic, because if i didnt change it, the top view and bottom view does not change.

2. As for the adjacent face, i hard code it to rotate each cell accordingly for a top row rotation. thus putting each cell on its respective next cell.

### Step 3: Use the same concept on the other rotation
1. Created rotateBottom() [the bottom row rotation], rotateLeft() [the left column rotation]. rotateRight() [the right column rotation]

2. the setState() was created for all rotations, following the given setState() code for rotateTop() also setState() for resetting the cube

### Step 4: Adding the buttons
1. I add the reset button on top right on the appbar

2. In the body, i add the other view other than the one provided, being the bottom face and rear face.

3. the next column, i made the 2 buttons, rotateTop and rotateBottom (The row rotations)

4. the next column, i made the other 2 buttons, rotateLeft and rotateRight (The column rotations)

That concludes the ways i did to make the rubik's cube.

