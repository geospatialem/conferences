# Git: Girl Develop It, October 2015 (Blomington, Minn.)

<img src="https://cloud.githubusercontent.com/assets/5023024/10260841/9d4cb9b8-6944-11e5-8987-a7d1493b5812.jpeg" width="25" height"25"> [Girl Develop It](http://www.midwestjs.com) is a non-profit organization that exists to provide affordable and judgment-free opportunities for women interested in learning web and software development. Through in-person classes and community support, Girl Develop It helps women of diverse backgrounds achieve their technology goals and build confidence in their careers and their every day lives.

## Introductions
* Presenter: [Amy Gebhardt](http://www.twitter.com/amlyhamm)
* [Presentation Slides](http://amlyhamm.com/gdi/fall_in_love_with_git)

## Vocabulary
* **_Repo_**: project folder (Git leprechauns).
* **_Clone_**: A copy of the Repo.
* **_Git_**: A program to track your Changes.
* **_Hashed commit_**: Unique IDs for commits (GitHub does this).
* **_Add_**: Add a file, or files, to the repository to be tracked.
* **_Stage_**: Tell Git to track the current state of the file.
* **_Commit_**: Saves the changes made to a file, not the file as a whole. The commit will have a "hash" so we can track which changes were committed when and by whom.
* **_Branch_**: A parallel version of a repo.
* **_Master_**: Default branch name on GitHub.
* **_Remote_**: Version of a repo on GitHub.
* **_Fetch_**: Get the latest changes from an online repo without merging (`git fetch`).
* **_Pull_**: Fetch and merge from the remote repo.
* **_Push_**: Send commits to the remote repo.
* **_Fork_**: A personal copy of another user's repo.
* **_Pull Request_**: Push your local changes to another user's repo, in hopes they will pull your code request to their repo to benefit others!
* **_Touch_**: Creates a new file (e.g. `touch .gitignore`).
* **_SSH Keys_**: Like a fingerprint, adds extra security to your GitHub account.

## Shortcuts
* Hit the `^` arrow to get the last run command in Terminal.
* Click `Tab` to finish the word/phrase you are typing.

### Tidbit
When you run into  `VIM` (text editor), do the following (also noted in [this StackOverflow message](http://stackoverflow.com/questions/14046122/github-locks-up-mac-terminal-when-using-pull-command)):  
1. Press `i`, a.k.a. insert, to insert the necessary message.  
2. Enter in the message necessary (no quotes, straight up text here is legitimite).  
3. Press `esc` to get to the prompt and then one of the following:  
a. `Shift` + `Z` + `Z`, or  
b. `:wq` (which is 1970's technology that means `w`: write, `q`: quit).  

## Version Control
Benefits include: collaborative environment, and the ability to track changes over time (esp. with groups of people)!

### Types
* Centralized
* Distributed (e.g. GitHub)

## Clone a Repo
### Straight up
`git clone [remote-location]`

### Rename the clone
`git clone [remote-location] [clone-name]`

### Project remotes
`git remote -v`

## How To Make a Repo

### 1. Create a Repo
To create a repo straight on GitHub, use the web tools to create one. There is a download option that can make repos with the command line named Hub. Check it out to learn more.

To create a repo on you desktop, without first making one on the web browser, run the following commands in Terminal:  

`mkdir [repo-name-here]`  
`cd [repo-name-here]`  

### 2. Initialize
`git init`  
`git status`  

### 3. Add a new file
`git add [file-name-here.ext]`  

## Undo Your Changes
Nobody's perfect. Sometimes you'll want to "undo" or "revert" some changes you've made.

Also, check out some awesome tweets that Nathan sent out! Such as [Git Alias'](https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases). Get all the information from the [Twitter discussion](https://twitter.com/GeospatialEM/status/649747875962875904).

P.S. **_AMAZING!_**

### Unstaged files
`git checkout [file-name-here]`  

### Staged files
`git reset HEAD [file-name-here]`  
`git checkout [file-name-here]`  

### Revert to a specific commit
Copy from Terminal and/or GitHub website, then run the following in Terminal:  
`git revert [commit-hash-here]`  

## Branches
A parallel version of a repo. `master` is GitHub's default branch. **A branch is a new ending to a novel.** Also, think of branches like components of a tree, like a tree branch!  

1. Same repo, with hopes of adding a new story in.  
2. `master` branch is left alone when doing large changes. Changes are normally merged into the `master` when completed.
3. Merge in a branch when you are ready, and after you have verified it works (usually back to the `master` branch).

### Create a Branch
`git checkout -b`  
`git status` will tell you the branch that you are in.

### Switch Branches
`git branch`: See all branches in the repo.   
`git checkout master`: Checkout the `master` branch.  

### Delete a Branch

**Origin Remote**:  
`git push origin :[branch-name-here]`  

**Locally**:  
`git branch -d [branch-name-here]`  

### Delete the Master (`master`) branch, and add a GitHub pages (`gh-pages`) branch  
1. Create the *gh-pages* branch locally (your machine), and switch to the branch:  
`git checkout -b gh-pages`  
2. Push the *gh-pages* branch to the origin (on GitHub):  
`git push origin gh-pages`  
3. Add the remote, or connection, between your origin and local copies:  
`git remote add gh-pages`  
4. Delete the origin *master* branch (on GitHub):  
`git push origin :master`  
5. Delete the *master* branch locally (on your machine):  
`git branch -d master`  

### Merge a Branch
a.k.a. collaboration at its best!

1. **Checkout the Branch** `git checkout master`. The branch you checkout will be the one you will be merging your changes to.

2. **Merge a Different Branch**: `git merge [branch-name-here]`. The branch you merge is what will be added to the branch you have checked out! **_WOOT!_** P.S. `git rebase` also works, but was not covered during our session.

### Branch Conflicts
Git will make you resolve conflicts before merging. When you try and run a merge and run into conflicts your file will change to show you the conflicts in your file(s). From here, edit them as you wish for them to appear. Then use `git commit -m '[your message goes here]'` to commit the changes. **_Hooray!_**

## Fork/Forking
Use/Contribute to a repo owned by someone else. Forking creates a personal copy in your account of someone else's repo. A fork makes it easy for you to modify the code, and for contributions, if the owner chooses to accept your changes.

## Pull Requests
After forking and cloning, any changes you push will go to **your local repo** (not the original repo you forked). However, you can contribute back to the original repo by submitting a pull request to the owner.

There is also a way for you to commit your changes **and** submit a pull request simultaneously using some awesome Git commands. Check out the GitHub Help section for more information on this awesomeness.
