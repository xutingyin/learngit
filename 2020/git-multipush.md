# Git 同时推送Github、Gitee

在你clone下来的项目根目录的.git[此文件夹为隐藏文件夹，如何显示，自行百度]文件夹内，找到config配置文件，添加你需要进行关联的远程地址：

```
[remote "gitee"]
	url = https://gitee.com/xutingyin/learngit.git
	fetch = +refs/heads/*:refs/remotes/gitee/*
	tagopt = --no-tags
[remote "github"]
	url = https://github.com/xutingyin/learngit.git
	fetch = +refs/heads/*:refs/remotes/github/*
	tagopt = --no-tags 
```

如果你还有其它的自己搭建的服务器地址，例如Gitlab等地址需要一起同步上去，就在config 配置文件中，按照上述方法配置即可。