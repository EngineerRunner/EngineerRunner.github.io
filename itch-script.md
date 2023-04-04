# ItchScript - a scratch programming language

Itch Script is an interpreted, function-based programming language (Heh, you think you're so cool with object-oriented programming languages), mainly designed for S-DOS (although a PC interpreter is coming soon).
This page has all the syntax you'll need to use it.
*Everything's a function!™*

## Basics

Generally, you use a > to show the start of an argument. Exceptions to this are listed in the section for each block, listed below.
There is a global "temporary variable". This acts like a "return" in other programming languages, and is used by everything. This temporary variable is accessible in most scripts by calling "temp" as a parameter.
On this page, // means a comment.

## Functions

### print

Prints text to the output prompt. Usage:

    print>Hello World
    print>temp //prints the temporary variable

### cmdshow

Shows the command prompt. If the command prompt is hidden and you can't enter this, tap this out on your keyboard (each direction is an arrow key):

    up, up, down, down, left, right, left, right, B, A

### cmdhide

Hides the command prompt.

### hello

Returns "world". Used for testing.


### equalto
Sets the temporary variable to true or false, depending on whether both arguments are equal.
Example:

    equalto>temp>1 //if the temp variable is one, this will set temp to true.

### runif
Runs the first argument as code, if the value is true. Evaluates argument 3 for seeing whether it's true. This block is very complicated, but here's a quick look at the syntax. (This would be all on one line, but it is indented to make it easier to read.)

    runif>
	    print; hello world> // inside this code, semicolons are used to seperate arguments. the print is what is run.
	    equalto; temp; 2 //the block will run if the temp var is set to true, which the equalto will do if both are equal.
This example on one line would be:

    runif> print; hello world> equalto; temp; 2
 
 I told you it was complicated!

### runifelse
Same as runif, but it runs argument 7 if the value is false.
### add
Adds 2 arguments together, and writes it to temp.
Usage:

    add> 1> 2

### subtract
Subtracts Argument 2 from Argument 1, and writes it to temp.
Usage:

    subtract> 47> 92

### multiply
Multiplies Argument 1 by Argument 2, and writes it to temp.
Usage:

    multiply> 5>7534

### divide
Divides Argument 1 by Argument 2, and writes it to temp.
Usage:

    divide> 5>7534

### varget
Gets a variable from the global variable list and writes it to temp. If the variable doesn't exist, this returns 0.
Usage:

    varget> variable-name

### varset
Sets a variable from the global variable list to a value, and, if it doesn't exist, creates it.
Usage:

    varset> variable-name> value

### input
Uses Scratch's "ask and wait" block. Sets a variable in the global variable list, the answer variable, to the value entered by the user. Also sets the temp variable to the answer.

### storetemp
Stores the temporary variable to another accessible variable. Unlike variables in the global list, this can directly be used as a parameter of a function. This variable is accessible with the keyword **stored**. (If you haven't seen already, the keyword for the temporary variable is **temp**.

### restoretemp
Sets the temporary variable to the stored variable.
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
### pendelete
Clears the pen canvas.
## Program Loading
You can now load apps!

 1. Enter command "loadstart" to show the list.
 2. See inside the project.
 3. Right click the list that was shown and import the file.
 4. Type loaddone.
 5. Enjoy!
# Features planned:
## More extensions
Sound (using the music extension), Online, and more.
## Planned Blocks/Features
 - Custom Functions - make your own function
 - Custom Extensions - make an extension!
# SPRITES WILL NEVER BE ADDED, AT LEAST IN THE TRADITIONAL, SCRATCH WAY.
