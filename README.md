# Pushing to Git
All future assignments will be submitted through Github instead of ICON. This assignment will help you get set up with pushing to Github. It must be finished by the end of Friday (11:59pm) to get credit for the quiz.

## Objective
To get credit, you need to do 2 things:
1. Change `test.cpp` by uncommenting the `cout` statement from `main`.
2. Add a file called `test.txt` with one line in it that just says "Hello, world" (no new line at the end).

## Instructions

### Clone
1. If you are part of the class organization `uiowa-cs-3210-spr24`, (which you should be after homework 1), following the invite link to the repo will create a private repository for you under the organization.
2. Until now, we were only dealing with public repositories, but when dealing with private repositories, Github requires that you use personal access tokens (PATs) for authentication instead of your Github password.
   Follow [these](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens) instructions to create a (classic) PAT and give it repository access. Store the PAT 
   somewhere safe and accessible, you will need it to clone the repo, pull from it, and push to it.
3. Now `clone` your private repo for quiz 03-04 (see instructions from homework 1 if you don't know how to do this) to your Desktop. Enter your Github username, and your PAT for the password.

### Commit
A commit stores changes made by you to the repo locally, and can be pushed to the remote repo. You'll need to commit your changes before pushing them.
1. Make the changes as specified in the [Objective](#objective) section.
2. Before committing, any new files must be added. In this case, you will need to add `test.txt`. You can add a file using `git add PATH_TO_FILE`. Specifically:
    ```
    git add test.txt
    ```
3. Now commit your changes:
   ```
   git commit -a -m "COMMIT_MESSAGE"
   ```
   Replace `COMMIT_MESSAGE` with a meaningful message that describes what this commit does.

### Push
Now we're ready to push our local changes to the online repo. Always pull before you push, in case the remote repo has been changed before your local changes are made:
```
git pull
git push
```
You'll need to authenticate with your Github username and PAT for both pulling and pushing since this is a private repository.
