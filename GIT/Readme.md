- To show the "full" help for a command: <br/>
  `git help [command]` <br/>
   eg: `git help init`  <br/>
- Setting your user name and email: <br/>
  `git config --global user.name "Dimple0501" ` <br/>
  `git config --global user.email "dimple@example.com"` <br/>
- Read your user name and email  
  `git config user.name` output **DimpleB0501** <br/>
  `git config user.email` output **dimple@example.com** <br/>
- Initialize (create) a repository in a folder
  `mkdir repos`<br/>
  `cd repos`<br/>
  `mkdir myproj`<br/>
  `cd myproj`<br/>
  `git init` __Initializes an empty git repository in myproj/.git/__<br/>
  `ls -a`   __will show a .git folder__<br/>
- Commit to local repository
  - `git status` view the status of files in the working tree and staging area.<br/>
  - `git add .` adds all untracked or moldified files using **git add .**. Or `git add <file or directory>` example `git add fileA.txt` or `git add dirA` <br/>
     **git add** adds untracked or modified files to the staging area.
  - `git commit -m "commit message" <br/>
     commit message syntax `<type>[optional scope]: <description>` <br/> 
     Allowed <type> values:<br/>
      feat (new feature for the user, not a new feature for build script)<br/>
      fix (bug fix for the user, not a fix to a build script)<br/>
      docs (changes to the documentation)<br/>
      style (formatting, missing semi colons, etc; no production code change)<br/>
      refactor (refactoring production code, eg. renaming a variable)<br/>
      test (adding missing tests, refactoring tests; no production code change)<br/>
      chore (updating grunt tasks etc; no production code change)<br/>
    **git commit** creates a snapshot of the current project.
   - **git log** can be used to view the commit history.
  
- Clone a remote repository
 `git clone <url/to/projectname.git>`
- Remote repository information
 `git remote -v`
- Adding a remote repository
  `git remote add <name> <url>`
- Push a commit to a remote repository
  `git push [-u][<repository>][branch]` <br/>
   - <repository> can be a name(shorcut/alias) or URL
   - `-u` track this branch
   - you can get your current *[branch]* with `git status`.
 - Adding commits - starting with no local repository
   - `git clone https://me@bitbucket.org/me/repoa.git`
   - cd repoa
   - echo "# My project's README" >> README.md
   - git add README.md
   - git commit -m "Inital commit"
   - git push -u origin master
-  The stash is a stack you can stash your changes at different branches by `git stash`. However to reapply. You have to push the index of the change you want to apply by `git stash pop stash@{n}` or `git stash apply stash@{n}`
- Branch in GIT 
  - Create the branch on your local machine and switch in this branch
    `git checkout -b [name_of_your_new_branch]`
  - Change working branch
    `git checkout [name_of_your_new_branch]`
  - Push the branch on github
    `git push origin [name_of_your_new_branch]`
  - See all branches created
    ` git branch`
  - Add a new remote for your branch
    `git remote add [name_of_your_remote] [name_of_your_new_branch]`
  - Push changes from your commit into your branch:
    `git push [name_of_your_new_remote] [url]`
  - Update your branch when the original branch from official repository has been updated:
    `git fetch [name_of_your_remote]` Then you need to apply to merge changes, if your branch is derivated from develop you need to do:
     `git merge [name_of_your_remote]/develop`
  - Delete a branch on your local filesystem :
    `git branch -d [name_of_your_new_branch]`
  - To force the deletion of local branch on your filesystem :
    `git branch -D [name_of_your_new_branch]`
  - Delete the branch on github :
    `git push origin :[name_of_your_new_branch]`
  The only difference is the : to say delete, you can do it too by using github   interface to remove branch : https://help.github.com/articles/deleting-unused-branches.
  - If you want to change default branch, it's so easy with github, in your fork go into Admin and in the drop-down list default branch choose what you want.
  - You want create a new branch: `git branch <name_of_your_new_branch>`
- To make sure your branch is up-to-date with the master
  `git checkout master`
  `git pull upstream master`
  `git checkout <ur branch>`
  `git merge master`
- Switching branches
  `git branch (displays all branches affilitated with you)`
  `git checkout <branch> (which branch you want to work on)`
- Removing a remote locally
  `git remote rm [<alias>]`




 
  
   

