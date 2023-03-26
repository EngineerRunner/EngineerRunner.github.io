# ItchScript - a scratch programming language

Itch Script is an interpreted, function-based programming language (Heh, you think you're so cool with object-oriented programming languages), mainly designed for S-DOS (although a PC interpreter is coming soon).
This page has all the syntax you'll need to use it.
*Everything's a function!™*
# NOTICE: RUNNING A PROGRAM FROM A FILE IS NOT YET SUPPORTED. IT IS JUST A COMMAND PROMPT FOR NOW.

## Basic Syntax

Generally, you use a comma to show the start of an argument. Exceptions to this are listed in the section for each block, listed below.

On this page, // means a comment.

### print

Prints text to the output prompt. Usage:

    print, Hello World
    print,temp //prints the temporary variable

### cmdshow

Shows the command prompt. If the command prompt is hidden and you can't enter this, tap this out on your keyboard (each direction is an arrow key):

    up, up, down, down, left, right, left, right, B, A

### cmdhide

Hides the command prompt.

### hello

Returns "world". Used for testing.


### equalto
Sets a temporary variable to true or false, depending on whether both arguments are equal. **(do not rely on this variable, as it is used globally. Use the setvar function to set a var to this value.)**

### runif
Runs the first argument as code, if the value is true. This block is very complicated, but here's a quick look at the syntax. (This would be all on one line, but it is indented to make it easier to read.)

    runif,
	    print; hello world, // inside this code, semicolons are used to seperate arguments. the print is what is run.
	    equalto, 1, 2 //the block will run if the temp var is set to true, which the equalto will do if both are equal.
This example on one line would be:

    runif, print; hello world, equalto, 1, 2
 I told you it was complicated!

### add
Adds 2 arguments together.
Usage:

    add, 1, 2

### varget
Gets a variable from the global variable list. If the variable doesn't exist, this returns 0.
Usage:

    varget, variable-name

### varset
Sets a variable from the global variable list to a value, and, if it doesn't exist, creates it.
Usage:

    varset, variable-name, value

### input
Uses Scratch's "ask and wait" block. Sets a variable in the global variable list, the answer variable, to the value entered by the user.

## Pen Blocks

There's also pen blocks, to be used in conjunction with cmdhide.


### pendown
Places the pen down.

### penup
Pulls the pen up.

### pentox
Moves the pen to an X position, and draws a straight line between the points if the pen is down.

### pentoy
Same as pentox, but for a Y coordinate.

### pentoxy
Same as pentox/pentoy, but does both at once. Argument 1 is X, Argument 2 is Y.
### pensettings
Just the "set pen () to ()" block from Scratch. Argument 1 can be colour, saturation, brightness or transparency, and Argument 2 is a value from 0 to 100.

# Features planned:
## More extensions
Sound (using the music extension), Online, and more.
## Planned Blocks/Features

 - runifelse - Just runif but also runs something else if the value is false.
 - subtract, multiply, divide
 - Custom Functions - make your own function
 - Custom Extensions - make an extension!
 - More temporary variables, for runif and other similar blocks.
 - Loading from a file.
# SPRITES WILL NEVER BE ADDED, AT LEAST IN THE TRADITIONAL, SCRATCH WAY.
