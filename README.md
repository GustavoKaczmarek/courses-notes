# Studying Notes

## Overview
This repository will contain all the necessary information so that I can remember how to program


## (Example )Pushing a repository from Git to GitHub
On the current folder, after creating the SSH connection between the computer with the remote repository. Copy the reference of the repository, for example: `git@github.com:GustavoKaczmarek/courses-notes.git` and paste it together with this command
```bash
git remote add origin git@github.com:GustavoKaczmarek/courses-notes.git
```

Then you can display the names of the remote repositories (like 'origin') that you have configured for your local repository, along with their associated URLs.

```bash
git remote -v
```

The output might look like:
```plaintext
origin  git@github.com:username/repository.git (fetch)
origin  git@github.com:username/repository.git (push)
```

Finally with the command `git push -f origin main` we upload our local branch commits to our remote repository. `-f` or `--force` is telling Git to forsce push the changes. Typically `origin` refers to the main remote repository associated and `main` specifies the branch I am pushing to on the remote repository.
