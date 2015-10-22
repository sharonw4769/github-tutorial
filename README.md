# GitHub Tutorial  
_by Sharon Wong_

---
## Git vs. GitHub
**Git** is the version control that keeps track of all changes made  
Git _does not_ require Github  
**Github** is a collaborative site that stores code and visually keeps track of any changes made  
Github _does_ require Git  
**_Github is similar to Git, however, Git can be used to keep track of changes as well as any errors or bugs_**

---
## Initial Setup
1. Go to [Github](http://www.github.com) website
2. Create an username and password
3. Select FREE plan
4. You now have a Github account!  

**HTTPS** stands for (**H**ypertext **T**ransfer **P**rotocol **S**ecure) requires the user to enter login information _EVERY TIME_  
**SSH Key** (**S**ecure **Sh**ell) does not require the user to enter login information

1. Log in onto Github
2. In settings (on the left side) select SSH key 
3. Click 'Add SSH Key' 
4. Add title and copy the SSH key (starts with ssh-rsa) from where you want to link (in this case, we are using Cloud 9)
5. Open IDE and type in `ssh -T git@github.com` then type in "yes"  

`git config` (to set up login information [user.name and user.email]): used when collaborating on projects in order to get credit for your contribution  
#### The code to submit your login information is:  
`git config --global user.name “First Last”`  
`git config --global user.email “Email Address”`

---
## Repository Setup
#### Create the directory by following these steps:   
1. In IDE, type in `mkdir (insert the name of file)`  
2. Go inside this folder by typing in `cd (whatever is the name of the file)`  
3. Type `git init` to initialize and create the first repository (this is usually done once in making of a directory)  
4. Put in login information using `git config`  
`(--global user.name “First Last”) (--global user.email “Email Address”)`  
5. Once the directory is created, add a new file (e.g. README.md) and once you open this file, you can add and edit the text inside   

#### IMPORTANT: Save/Add/Commit  
- Save any changed made (_Auto-save_ is **recommended**)  
- Use `git add [file]` in order to add any file(s) 
- Use `git commit -m "(message)"` to display a mini message  

#### Making a new repo on Github  
1. On your Github account, (top right) there is a (+) sign that allows you to create a new repository
2. Press on "New Repository" and then fill out the folder information  

#### What is a remote?
* A remote is used to link the repository to Github so that it can be visually presented live

---
## Workflow & Commands
`git status` is used to make sure there is no errors in the code   
- (frequent use of this command is **recommended**)

#### The Process of _adding, committing,_ & _pushing_ 
* `git add`: add any 'new' file(s)  

**3 ways to add files**  
1. `git add [file(s)] ` - add committed file(s)   
2. `git add --all` - add ALL files  
3. `git add .` - add everything


* `git commit -m "(message)"`: allows user to add a short/specific message so they can refer back to this change (message should be _present-tense_ and specifically describe and answer _What work/change was done_?) 
* `git push -u`: send committed changes from local repository to remote repository (Github)  
The `-u` stands for "upstream" which will remember where to push the changes to (done once and then you can use `git push`) 

---
## Error Handling
If by any chance, you intialized (`git init`) the wrong directory, just `cd` to get out of where you currently are (you can cd back into main folder by doing `cd ..`) and them type in `rm -rf (folder name)` to forcefully removes the file/directory. 