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
git checkout name

或者
git switch name

例如 

    git checkout master

合并分支
---
    git merge dev
注：如果需要将B分支合并到A分支，则应该切换到A分支，再 git merge B
我在合并分支后，发现需要再进行 push,A 分支上才有合并后的内容，不然是合并前的A分支内容

    git push origin master

分支管理策略
--
Fast Forward（默认是这种策略）

Recursive（通过 --no-ff 即可使用禁用 Fast Forward策略，使用此策略）

回退
--
git reset --hard HEAD^         回退到上个版本

git reset --hard HEAD~3        回退到前3次提交之前，以此类推，回退到n次提交之前

git reset --hard commit_id     退到/进到 指定commit的sha码
