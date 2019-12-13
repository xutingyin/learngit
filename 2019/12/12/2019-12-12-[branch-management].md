# 分支管理
##前言

灵魂拷问--为什么我们需要分支？

![git-branch](images/git-branch.png)

上面的图很好的解释了这个问题，我们可以像悟空分身一样，不同的分支做不同的事情，最后将所有的分支进行合并，这样就啥都会了。

## 查看分支
	git branch     // 查看本地分支
	git branch -r  //查看远程分支
	git branch -a  //查看所有分支

##创建分支

方式1：

	git checkout -b dev

方式2：

	git branch dev 
	git checkout dev

## 合并分支
场景：需要将dev 上的代码合并到master主干分支上

操作：

	git checkout master  // 首先切换到master分支
	git merge dev		 // 将dev 分支合并到master分支

## 删除分支
本地分支删除： git branch -d dev

远程分支删除： git push origin -delete dev


