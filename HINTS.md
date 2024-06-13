# HINTS

## Git Command Rundown
- `git status` - Shows the current status of any local changes
- `git log` - Shows the log of all previous commits
- `git add .` - Adds all local changes to the staging area
- `git add fileNameHere` - Adds only the specified file to the staging area
- `git commit -m "commit message here"` - Creates a commit of all currently staged changes and adds the commit message to the log
- `git push` - Pushes all local commits to GitHub and creates a new Pull Request for review (if a Pull Reqeust already exists, this command will just update the existing Pull Request with the new commits you pushed)
- `git pull` - Pulls all changes from the repo to the local machine
  - NOTE: To avoid confusing issues, please make sure you're on the *main* branch when you run this command
- `git branch branchNameHere` - Creates a new branch named branchNameHere
  - NOTE: This command will only _create_ the new branch. The following command is how you actually switch to that branch.
- `git checkout branchNameHere` - Switches from the current branch to branchNameHere
- `git checkout -B branchNameHere` - Creates a new branch named branchNameHere and switches to it
  - NOTE: This creates the new branch off of the _current_ branch. For our purposes please make sure you're on the *main* branch before running this command

## General Hints
- To keep things simple and clean for now, always make new branches off of the main/master branch
- Remember our visualization of three boxes when you're figuring out how to get local changes to GitHub for review:
  -  "Staging" -> "Committed" -> "GitHub"
- `git status` will show you what branch you're currently on
- Only staged changes will be committed when you use the `git commit` command; unstaged changes will not be included in the commit
- Only changes in a commit will be pushed to GitHub for review
- Your local copy of the main branch _does not_ automatically remain up-to-date with the main branch in the GitHub repo; you must specifically _pull_ in any changes which exist in the repo
- After your Pull Request is approved and you click the Merge button, the code changes in the Pull Request are merged into the master branch in GitHub