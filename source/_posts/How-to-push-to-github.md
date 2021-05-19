---
title: How to push to github
date: 2021-03-05 21:39:09
categories: [git,github]
tags: [git,github]
---

之前刚开始接触Github的时候，有太多需要注意的点需要care，所以很多时候都畏手畏脚，导致有许多次想要尝试却铩羽而归，这次就以如何push自己的项目到github仓库上举例

# 本文将介绍如何将自己的项目push到github上，如何及时发布自己项目的每次更新

<!-- more -->

![](https://github.com/sujit-168/Blog-Picture/raw/master/My%20Blog/How-to-push-to-github/push%20to%20github.jpg)

```
git checkout -b dev #创建一个名为dev的新分支并切换到该分支，如已有dev分支，去掉-b即可切换到dev分支
git add .  # 增加改动
git commit -m "first commit"  # 提交本次名为first commit的修改
git pull  # 如果出现冲突，则需要执行此代码
git log -p # 查看本次提交所进行的修改，确认无误即可进行下一步操作
git push origin dev
```

![](https://github.com/sujit-168/Blog-Picture/raw/master/My%20Blog/How-to-push-to-github/Screenshot%202021-03-05%20221546.jpg)

然后就会在你所提交的仓库中出现一个新的New pull request请求（也就是分支合并请求）

![](https://github.com/sujit-168/Blog-Picture/raw/master/My%20Blog/How-to-push-to-github/pullrequest.jpg)

拉取本次pull request请求

![](https://github.com/sujit-168/Blog-Picture/raw/master/My%20Blog/How-to-push-to-github/request.jpg)

设置assigners，label等信息

![](https://github.com/sujit-168/Blog-Picture/raw/master/My%20Blog/How-to-push-to-github/set.jpg)

点击merge （合并）本次pull request

![](https://github.com/sujit-168/Blog-Picture/raw/master/My%20Blog/How-to-push-to-github/merge.jpg)

本次push to github完成

![](https://github.com/sujit-168/Blog-Picture/raw/master/My%20Blog/How-to-push-to-github/ok.jpg)

## OK！本期关于如何将自己的项目Push到github上就到此为止。喜欢的话请支持、转发、订阅！同时也欢迎各位大佬指出不足之处！在此本人万分感谢！