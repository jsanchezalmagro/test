# Git clone parcial
``` cmd
mkdir <repo>
cd <repo>
git init
git remote add -f origin <url>

git config --local core.sparseCheckout true

echo "some/dir/" >> .git/info/sparse-checkout
echo "another/sub/tree" >> .git/info/sparse-checkout

git pull origin <branch>

```
- with gitextensions create a empty repsitory
- after add remote repository
- configuration git with option "git config --local core.sparseCheckout true"
- create the file ".git/info/sparse-checkout"
- add to "sparse-checkout" the directories to include
- git pull over branch
