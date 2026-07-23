Matt Brigidi | Sr. Director, Innovation & Solutions | 2026-07-23
***

After [pulling the most up-to-date](/languages/git/c_how_to_start_working.md) version of the repo, you'll want to create a new branch.

## how to create a new branch
you'll want to use the following command:

```shell

git switch -c "action/branch_name_goes_here"

```

## how to structure your branch name
you're encouraged to have two components to your branch structure

1. the action you are taking
2. a brief descriptor to help understand what happened in the branch

## what options to use for the 'action' portion
the action portion is meant to identify what the reason for the branch is. the following are some examples of some `flags` you might use:

| action option | what it means |
| :---: | :---: |
| addition | something is being added to the code base |
| issue | something is being changed because of an error-adjacent consideration |
| refactor | something is being changed that existed, and it will continue to exist just differently |

## how to handle branch names
you'll want to keep them short. they should try to add value, so that you and your peers can understand what happened. remember that you'll also have commits to denote the changes, so the branch name is the "title", while the commits are the chapters, and the code is the story. 
