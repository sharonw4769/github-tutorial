# GitHub Tutorial  
_by Sharon Wong_

---
## Git vs. GitHub
**Git** is the version control that keeps track of all changes made  
Git _does not_ require Github  
**Github** is a collaborative site that stores code and visually keeps track of any changes made  
Github _does_ require Git  
** _Github is similar to Git, however, Git can be used to keep track of changes as well as any errors or bugs_**

---
## Initial Setup
1. Go to [Github](http://www.github.com) website
2. Create an username and password
3. Select FREE plan
4. You now have a Github account!  

HTTPS stands for (**H**ypertext **T**ransfer **P**rotocol **S**ecure) requires the user to enter login information _EVERY TIME_  
SSH Key (**S**ecure **Sh**ell) does not require the user to enter login information

1. Log in onto Github
2. In settings (on the left side) select SSH key 
3. Click 'Add SSH Key' 
4. Add title and copy the SSH key (starts with ssh-rsa) from where you want to link (in this case, we are using Cloud 9)
5. Open IDE and type in `ssh -T git@github.com` then type in "yes"  

`git config` (to set up login information [user.name and user.email]): used when collaborating on projects in order to get credit for your contribution  
The code to submit your login information is:  
`git config --global user.name “First Last”`  
`git config --global user.email “Email Address”`

---
## Repository Setup
`init`  
first `add` & `commit`  
new repo on github  
remote


---
## Workflow & Commands