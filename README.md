# com.mishra.dev.docs
Documentation related to com.mishra.dev.* projects.

Code organization.

com.mishra.dev.root has the root POM. All dependencies and their versions should be defined here. This project should be referenced in all com.mishra.dev* projects. 

com.mishra.dev.tools has the tools related to checkstyle, findbugs and other standards that should be applied to all com.mishra.dev* projects.

Any com.mishra.dev* project will ideally include both com.mishra.dev.root and com.mishra.dev.tools projects as maven dependencies.

Simple Git Starter.

Download git client for your OS from here 
https://git-scm.com/downloads

Go to terminal or git bash command prompt (if you are on Windows).
Run command: git --version

Use the following guide to setup git for github 
https://help.github.com/articles/connecting-to-github-with-ssh/

Typically it requires you to
1. Create a key-pair
2. Upload the public key on github account.
3. Get going.

Development workflow.

Once your github access is setup- do the following from terminal/git bash.

Clone a repository -
example:
git clone git@github.com:mrabhishek/com.mishra.dev.root.git

Create a local branch for your changes.

git checkout -b "branch-name"
e.g. git checkout -b "feature/test-feature"

Now make changes to a file.

Find changes in your repository -

git status

You might see files in red or green. 
Files in red means that the changes are not yet staged. 

Add all changed files to staging area (no committing yet) -
git add -A
(you can add one file at a time by doing -
git add "file-name"

Once you added files verify that they show as green -

git status

Now it's time to commit -

git commit -m "my sample commit message"

Now you have commited the changes to your local copy.

It's time to push the changes to the source repository (the one on github)

git push origin "your branch name"
e.g.
git push origin feature/test-feature

Go to github and verify that a branch was pushed.
On github, click "Create a pull request" and follow directions to use the
recently pushed branch to create a pull request (PR).

