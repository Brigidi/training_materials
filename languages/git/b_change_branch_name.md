Matt Brigidi | Sr. Director, Innovation & Solutions | 2026-07-23
***

it's common practice for the primary branch in git to be called `main`. in some cases, legacy systems will default to `master`. 

## why the word main became best practice
historical context denotes negative connotation with the word `master`, so ppl switched to using `main`

# how to change the name of the branch
regardless of the name you choose — the following outlines how to change the name of a branch:

```shell

git branch -m master main
git push -u origin main

``` 

if you are using github, then you will be prompted with a link to the repo. 

1. go to the `Settings` menu item
2. in the `General` section, navigate to the `Default branch` sub-section
3. select the dropdown menu and switch the default branch from `master` to `main`

go back to your editor and enter the following command:

```shell

git push origin --delete master

```


