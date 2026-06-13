# command cheat sheet: shell
this file aspires to introduce some commands that will help you get you rooted when using the terminal window. 

## shell languages
there are variations of shell syntax, which means some of the commands listed in this repo might not 1:1 with language used by your machine and/or environment. if that's the case, you can use web-search and/generative ai to identify what is applicable to you.

## how to identify your shell language
open up your terminal interface and enter the following command:

```echo $SHELL```

the output will likely provide one of the following:

| output | language | common environments |
| :---: | :---: | :---: |
| /bin/zsh | zsh | macOS or linux |
| /bin/bash | bash | linux or servers |
| /bin/fish | fish | third-party shell |
| /bin/sh | sh | docker |

some words to know:

- "bash" stands for bourne-again shell
- "sh" stands for bourne shell

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
