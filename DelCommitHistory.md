Deleting the .git folder may cause problems in your git repository. If you want to delete all your commit history but keep the code in its current state, it is very safe to do it as in the following:

1.      If forked, rename repo in web browser
 

2.     
Cd into the local repo
cd path/to/repo
 
3.      Checkout
git checkout --orphan latest_branch
 
4.      Add all the files
git add -A
 
5.      Commit the changes
git commit -am "commit message"
 
6.      Delete the branch
git branch -D main
 
7.      Rename the current branch to main
git branch -m main
 
8.      Finally, force update your repository
git push -f origin main
 
PS: this will not keep your old commit history around
 
 
Thanks in advance,
 
 
Rob
 
ROBERT VANCE | Principal Security Architect, Information Security
My SLEEP NUMBER® setting is 75. What’s yours?
P 763.551.6917
robert.vance@sleepnumber.com
 
NOTE: Getting this email out of normal working hours? Most of us work at a digitally enabled relentless pace, which can disrupt our ability to sleep enough, eat right, exercise, and spend time with the people that matter most. I am sending you this email at a time that works for me. I only expect you to respond to it when convenient for you!
