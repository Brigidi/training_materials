Matt Brigidi | Sr. Director, Innovation & Solutions | 2026-07-23
***

if you accidently delete a branch, you can restore the file using the commit history and move it to a folder to manage it.

## how to find delete file path and commit
you can use this command to see your git log:

```shell

git log --all

```

additionally, you can also reference the file path:

```shell

git log --all --path/to/deleted/file.py

```

## how to restore the file
you can reference a specific commit using:

```shell

git restore --source=<commit_hash> 

```

similarily to the above, you can also reference the file path:

```shell

git restore --source=<commit_hash> --path/to/deleted/file.py

```

## what else you can do
this is a new thing for me, so i'll be filling it out as needed
