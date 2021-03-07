# git-orphaning

Given: "main" branch with 3 commits which should have been in branch "dev"
ToDo: move commits without losing your history
Solution:

git branch --move master dev
git checkout --orphan master
git rm -rf .
