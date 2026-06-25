# command cheat sheet: shell
this file aspires to introduce some commands that will help you get you rooted when using the terminal window. 

## shell languages
there are variations of shell syntax, which means some of the commands listed in this repo might not 1:1 with language used by your machine and/or environment. if that's the case, you can use web-search and/generative ai to identify what is applicable to you.

## how to identify your shell language
open up your terminal interface and enter the following command:

```
echo $SHELL
```

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

the following actions rerquire you to hold down the keys at the same time.

| keyboard input | terminal output |
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

**note**: the above is written from the use of ```zsh```, which means there might be some variance if your shell uses a different language.

## navigating your system
the following commands will help you identify where you are in your machine, as well as how to move around it.

| command | what it means | what it does |
| :---: | :---: |:---: |
| pwd | present working directory | shows the file path to the directory you are currently working in |
| ls | list | shows all directories and files in your present working directory |
| cd | change directory | allows you to move from your present working directory to another directory|

the ```ls``` and ```cd``` commands both have additional **flags** that provide additional functionality. in the case of ```cd``` you will learn how to move forward and backwards in the lessons ahead.

## directories
the following will outline some commands to manage directories (aka *folders*).

| command | what it means | what it does |
| :---: | :---: | :---: |
| mkdir | make directory | creates a new folder |
| rmdir | deletes directory | deletes an **empty** folder |

if you want to delete a folder but it has anything in it, then you will need to use a **potentially dangerous ** command. please be careful when using the following:

| command | what it means | what it does |
| :---: | :---: | :---: |
| rm -rf | remove recursively and forcefully | removes all files, sub-directories, and nested data |

the ```-f``` command will override safety prompts and write protected files. You will not be asked a follow-up question before removal; and the contents will not be retrievable via the "trash". 

the reasons ```rm -rf``` can be extremely dangerous is if you use it at lower-levels of your operating system. that doesn't mean you should not use the command; it merely means you should be mindful and intentional when using it.

## files
the following will outline how to manage files, which will be stored within your directories.

| command | what it means | what it does |
| :---: | :---: | :---: |
| touch | legacy word from early computing | creates a file |
| mv | move | allows you to move a file to a location in your system |
| scp | secure copy protocol | makes a copy of a file in a specified location |
| rm | remove | deletes a file from your system |

you can create file types the same way you would when using your gui. here is a breif overview of some file types you might want to create:

| type | notes |
| :---: | :---: |
| .txt | text file |
| .md | markdown file |
| .py | python file |
| .yaml | yet another markup language file |
| .csv | comma-separated value file |
| .json | java-script object notation file |
| .sql | structured query language file |

