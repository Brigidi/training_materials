Matt Brigidi | Sr. Director, Innovation & Solutions | 2026-07-23
***

after you push your branch to the repo on github via `pull request`, you will want to delete your branch from:

1. the github repo
2. your local git repo

this is called `pruning`

## why you prune branches
your changes should be merged into `main`, which makes those changes part of `prod`. you no longer need the branch. hypothetically, having old branches without pruning, could cause confusion about what branches are actively in development compared to ones that had been in development but were merged into `main`.

## how you prune branches
you'll want to push your branch to the github repo, so that your pull request can be reviewed:

```shell

git push

```

you will likely get a message that says something like:

```shell

fatal: The current branch NAME_GOES_HERE has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin NAME_GOES_HERE

```

you can copy this line of code

```shell

git push --set-upstream origin NAME_GOES_HERE

```

that adds your branch to the github repo. after the pull request is merged into `main`, you will delete the branch in github, and then return to your local repo and use the following command:

```shell

git switch main

```

that command will return you to main and then you can pull down the most up-to-date version of main from github:

```shell

git pull 


```

now, you can safely prune your development branch using:

```shell

git branch -d NAME_GOES_HERE

```
