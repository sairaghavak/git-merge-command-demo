# Quick `git merge` command demo

Part - I
---
1. Create a repo - by default it is `master` branch
2. Freeze a commit `m1` - milestone1

Part - II
---
1. Create a new `branch` called `b1-cut-from-commit-m1` from `master`
2. Freeze a commit `b1` - feature1 


|`master` commit messages stack | `b1-cut-from-commit-m1` commit messages stack|
|---|---|
|`m1`| `b1` <br> `m1`|
|Now assume there is a change made to master as `m2` and the new commit stack for master looks like below  <br> `m2` <br> `m1` | If we do `git merge master` from `this` branch. <br> Then <br> 1. It may result in conflicts. <br> 2. We have to fix those conflicts. <br> 3. Then do `git commit` <br> Now, the commit message stack for this branch looks like this <br> `Merge branch 'master' into b1-cut-from-commit-m1` <br>`m2` <br> `b1` <br> `m1`|


