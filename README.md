Git is a version control system.
Git is a free software.
I love git.
Git tracks changes of files
Git branch test.

创建分支
----------
    git checkout -b dev
git checkout -b dev 等价于执行了下面两条命令

    git branch dev
    git checkout dev

查看分支
---
    git branch

切换分支
--
git checkout branchname

例如 

    git checkout master

合并分支
---
    git merge dev
注：如果需要将B分支合并到A分支，则应该切换到A分支，再 git merge B
我在合并分支后，发现需要再进行 push,A 分支上才有合并后的内容，不然是合并前的A分支内容
    git push origin master