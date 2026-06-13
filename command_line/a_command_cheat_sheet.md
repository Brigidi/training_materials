# command cheat sheet: bash
this file aspires to introduce some commands that will help you get you rooted when using the terminal window. 

## moving the cursor
command-line does not allow you to point-and-click the same way a text-editing software does. that means the cursor (aka the "floating box") will not move if you attempt to click at different points of a line.

| keyboard input | **terminal output** |
| :---: | :---: |
| control-a  | returns the cursor to the start of the line |
| control-e | moves cursor to the end of the line |
| option-left arrow | moves cursor one word to the left |
| option-right arrow | moves the cursor one word to the right |
| control-u | deletes the entire line *or* deletes all input to the left of the cursor |
| control-y | pastes _everything_ you just deleted to the right of the cursor |
| control-k | deletes *all* input to the **right** of the cursor |
| esc-d | deletes the word to the **right** of the cursor |
| control-w | deletes the word to the **left** of the cursor |
