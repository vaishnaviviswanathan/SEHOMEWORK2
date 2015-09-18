# OS: Windows operating system  
# Software Used: Git Shell 
#The below commands were entered step by step to generate the tree  

mkdir SEHOMEWORK2
new-item README.md -file
git init

invoke-item README.md
git add README.md
git commit -m "commit 0"

invoke-item README.md
git add README.md
git commit -m "commit 1"

invoke-item README.md
git add README.md
git commit -m "commit 2"

git log

git checkout 71bffe05d137fb79ec2d714c93cc4f939227989f # ---> node 0
git checkout -b bug-fix

invoke-item README.md
git add README.md
git commit -m "commit 3"

invoke-item README.md
git add README.md
git commit -m "commit 4"

git merge master

# The previous command will create merging conflicts since the same line was changed twice.
#  " Auto-merging README.md
#   CONFLICT (content): Merge conflict in README.md
#   Automatic merge failed; fix conflicts and then commit the result."

invoke-item README.md
git add README.md
git commit -m "commit 5"

gitk #---> (to view the graph in Git shell)

invoke-item README.md
git add README.md
git commit -m "commit 6"

git log

git checkout 34f81895c30becb58d7121fb1203de33e22d8c03 #-->node 4

git checkout -b bug-fix-experimental

invoke-item README.md
git add README.md
git commit -m "commit 7"

invoke-item README.md
git add README.md
git commit -m "commit 8"

invoke-item README.md
git add README.md
git commit -m "commit 9"

git checkout master

invoke-item README.md
git add README.md
git commit -m "commit 10"

git checkout bug-fix

git merge bug-fix-experimental

invoke-item README.md
git add README.md
git commit -m "commit 11"


invoke-item  README.md
git add README.md
git commit -m "commit 12"

git checkout master
git merge bug-fix

invoke-item  README.md
git add README.md
git commit -m "commit 13"

invoke-item  README.md
git add README.md
git commit -m "commit 14"
