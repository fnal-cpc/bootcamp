# Preface

Some very useful general git/github tutorials can be found [here](https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners) or [here](https://guides.github.com/activities/hello-world/). Some tutorials by the cosmologist [Phil Marshal](https://github.com/drphilmarshall) can be found [here](https://github.com/drphilmarshall/GettingStarted).

# How to Git

Have you ever had a document that you keep making copies of with slightly different names (e.g., `v1`, `v2`,...)? If so, then `git` may be for you! `git` is a version control system that builds a repository (or `repo`) to track your documents and the changes that you make to them. This allows you to revert your changes to previous versions, as well as merge changes from your collaborators. In our general usecase, `git` allows you to work locally on a code base and then merge and upload your changes with a remote version of the code online. Think of `git` like  clone on a local system, then commit changes and upload (push) to a remote repository. 

There is a lot of jargon surrounding the use of `git`. You can create repositories ("repos"), "fork" (i.e., make your own copy) of an existing repository, "commit" your changes to the content of that repository, "push" (i.e., upload) your changes to the remote repository, and "merge" your changes with that repository. When working with `git` through GitHub, you can create and track "issues" or work with your collaborators to develop new code or fixing existing code.

## How does this work?

You initialize a repository using `git init .`. This starts `git` version tracking of the current directory. (If you are ever interested in seeing how the sausage is made, you can look in the `.git` directory that is created.) 
You create a new document as usual and commit `git commit -m "Some descriptive text" new_doc.txt`.
Add the remote path `git add remote https://github.com/GITHUB_ORG/GITHUB_REPO.git`
And once you are ready you can push `git push origin master`.


## Cloning

Git/GitHub allows you to "pull" (download) public code in your local machine, change that code and
contribute it back to the original codebase. On GitHub you can "fork" a repository (make your own personal copy on GitHub) by pushing the "Fork"  button, or you can "clone" a repository (grab a local copy on your machine) by pushing the green "Clone or download" button, copying the displayed path, and then in a terminal running the command: `git clone https://github.com/GITHUB_ORG/GITHUB_REPO.git`. After this you can
install the code, modify the code, etc. (As allowed by the code license).

## Branches

Git allows you to do parallel development in so-called "branches". Once you create a branch, you are able to make  modifications that don't affect the code in the other branches. After you finish making your changes you can
merge with the main branch (generally called the "master" branch) or any other branch using `git merge`.

## Pull request

Rather than directly merging, it is usually recommended to create a "pull request" (often abbreviated "PR") before merging branches. This operation allows you to compare the new additions in the branch, and even allows to generate a review process before proceeding to merge. 

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
