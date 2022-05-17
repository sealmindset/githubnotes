A very safe way to delete all your commit history but keep the code in its current state.

1. If forked, rename repo in web browser
 
2. Cd into the local repo

cd path/to/repo
 
3. Checkout

git checkout --orphan latest_branch
 
4. Add all the files

git add -A
 
5. Commit the changes

git commit -am "commit message"
 
6. Delete the branch

git branch -D main
 
7. Rename the current branch to main

git branch -m main
 
8. Finally, force update your repository

git push -f origin main
 
PS: this will not keep your old commit history around
