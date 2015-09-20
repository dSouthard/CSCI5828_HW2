# CSCI5828_HW2
Diana Southard, Fall 2015 <br>
<br>
List of commands used:<br>
<br>
##### Started Git Repo<br>
echo "# CSCI5828_HW2" >> README.md<br>
 git init<br>
git add README.md<br>
git commit -m "first commit"<br>
git remote add origin git@github.com:dSouthard/CSCI5828_HW2.git<br>
git push -u origin master<br>
echo "Commi 1" > masterbranch<br>
git add .<br>
git commit -m "Commit 1"<br>
echo "Commit 2" >> masterbranch<br>
git add .<br>
git commit -m "Commi 2"<br>
git push origin master <br>
git log --graph<br>
##### Start bug-fix branch<br>
git checkout ab4fb75cab376382acb1277c3d6d2caecaf39184<br>
git checkout -b bug-fix<br>
echo "Commit 3" > bugfix<br>
git add .<br>
git commit -m "Commit 3"<br>
echo "Commit 4" >> bugfix <br>
git add .<br>
git commit -m "Commit 4"<br>
git push origin bug-fix <br>
##### Merge bug-fix/master<br>
git merge master <br>
git log --graph <br>
echo "Commit 6" >> bugfix<br>
git add .<br>
git commit -m "Commit 6"<br>
git push origin bug-fix <br>
##### Start bug-fix-experimental branch<br>
git checkout 6a69f4e016bc412a3f879dcc50c280c69a68c5fa<br>
git checkout -b bug-fix-experimental<br>
echo "Commit 7" >> bugfix<br>
git add .<br>
git commit -m "Commit 7"<br>
echo "Commit 8" >> bugfix <br>
git add .<br>
git commit -m "Commit 8"<br>
echo "Commit 9" >> bugfix <br>
git add .<br>
git commit -m "Commit 9"<br>
git push origin bug-fix-experiment<br>
git log --graph<br>
git checkout master <br>
echo "Commit 10" >> masterbranch <br>
git add .<br>
git commit -m "Commit 10"<br>
##### Merge bug-fix/bug-fix-experimental<br>
git checkout bug-fix<br>
git merge bug-fix-experimental <br>
##### CONFLICT (content): Merge conflict in bugfix, Automatic merge failed<br>
git add .<br>
git commit -m "Commit 11"<br>
echo "Commit 12" >> bugfix<br>
git add .<br>
git commit -m "Commit 12"<br>
git push origin bug-fix<br>
### Merge master/bug-fix<br>
git checkout master <br>
git merge bug-fix<br>
### Put all the git commands used to create this repo into README.md<br>
git add README.md<br>
git commit -m "Commit 14"<br>































