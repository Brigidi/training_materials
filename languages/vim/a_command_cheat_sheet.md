# command cheat sheet: vim
this file aspires to provide some keyboard shortcuts that will help you when using the vim editor in terminal.

## modes
vim has a few modes, which change what shortcuts are available to you.

| mode | keyboard_command | explanation |
| :---: | :---: | :---: |
|normal mode | ```esc``` | default mode when entering vim. keys are commands |
| insert mode | ```i``` | this mode allows you to type and enter text |
| visual mode | ```v``` | this allows you to highlight and select blocks of text |
| command-line mode | ```:``` | this allows you to enter commands that change editor settings and save your progress |

to enter any of the modes, you hit the keyboard command listed above. you can exit the modes by hitting the ```esc``` key.

## navigation
the following commands will help you move around the editor space.

| action | mode | keyboard_command | what_it_does |
| :---: | :---: | :---: | :---: |
| jump to end of file | normal | ```shift```+```g``` | moves the cursor to the last character of the file |
| jump to start of file | normal | ```gg``` | moves the cursor to the very beginning of the file |
| move to the right | normal | right-arrow key or ```l``` | moves the cursor to the right |
| move cursor to left | normal | left-arrow or ```h``` | moves cursor to the left |
| move cursor up | normal | up-arrow or ```k``` | move cursor up |
| move cursor down | normal | down-arrow or ```j``` | move cursor down |
| move to end of line | normal | ```$``` | moves cursor to last character of current line |
| move cursor to front of line | normal | ```0``` | moves cursor to first character of current line |
| move cursor to next word | normal | ```w``` | moves cursor to first character of next word |
| move cursor to end of word | normal | ```e``` | moves cursor to last character of current word | 
| move cursor to previous word | normal | ```b``` | moves cursor to the previous word; it will also move cursor to the first character of the current word if not at the start of the word |

## text editing
the following will help you delete or replace words.

| action | mode | keyboard_command | what_it_does |
| :---: | :---: | :---: | :---: |
| delete from cursor to next word | normal | ```dw``` | deletes up to two words |
| delete the current line | normal | ```dd``` | deletes the whole line | 
| replaces a single character | normal | ```r``` + ```new_character``` | replaces the character underneath the cursor |
| undo what you did | normal | ```u``` | undo previous action | 
| redo previous undo | normal | ```ctrl``` + ```r``` | redo your undo |

 
