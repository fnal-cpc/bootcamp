# Preface

Some very useful git/github tutorials can be found [here](https://github.com/rmjarvis/GettingStarted)
and [here](https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners) or [here](https://guides.github.com/activities/hello-world/)

# How to Git

`Git` is a version control system. It allows you to work "offline" and clone on a local system,
then commit changes and upload (push) to a remote repository. It enables collaboration.

You can create repositories (repos), fork exisiting ones (i.e., make your own copy of a repo),
create issues, or collaborate including new code or fixing existing code.

## How does this work?

You initialize a repository using `git init .`. This starts the versioning.
Then you create a new document as usual and commit `git commit -m "Some descriptive text" new_doc.txt`.
Add the remote path `git add remote https://github.com/GITHUB_ORG/GITHUB_REPO.git`
And once you are ready you can push `git push origin master`.


## Branches

Git allows you to do parallel development in the so-called branches. Once you create a branch, the modifications
done there don't affect the code in the other branches, after you are done with your developments of a branch you can
merge with the master (or other branch) using `git merge`.

## Pull request

Rather than directly merging, it is usually recommended to create a pull request before merging branches. This operation
allows you to compare the new additions in the branch, and even allows to generate a review process before proceeding
to merge. 

## Hands on

**EXERCISE** Fork this repository and create a local clone. Then open an issue.

**EXERCISE** Find the bug in the `example_broken.py`. Create a new branch and create a pull request.


```
HINT:
git checkout -b patch1_branch
edit example_broken.py
git commit -m "Fixed example" example_broken.py
git push origin patch1_branch
```
