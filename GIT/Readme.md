- To show the "full" help for a command: <br/>
  `git help [command]` <br/>
   eg: `git help init`  <br/>
- Setting your user name and email: <br/>
  `git config --global user.name "Dimple0501" <br/>
  `git config --global user.email "dimple@example.com"` <br/>
- Read your user name and email  
  `git config user.name` output **DimpleB0501**
  `git config user.email` output **dimple@example.com**
- Initialize (create) a repository in a folder
  `mkdir repos`
  `cd repos`
  `mkdir myproj`
  `cd myproj`
  `git init` __Initializes an empty git repository in myproj/.git/__
  `ls -a`   __will show a .git folder__
- Commit to local repository
  - `git status` view the status of files in the working tree and staging area.
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
 -  the stash is a stack you can stash your changes at different branches by `git stash`. However to reapply. You have to push the index of the change you want to apply by `git stash pop stash@{n}` or `git stash apply stash@{n}`

 
  
   

