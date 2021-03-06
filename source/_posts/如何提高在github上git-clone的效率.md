---
title: 如何提高在github上git clone的效率
date: 2021-04-13 08:17:00
categories: [github]
tags: [github]
copyright: true
---


最近在github上clone一些机器学习的项目时，发现下载速度很慢，只有几kB/s，需要等待很久，才能下载完整个项目，并且途中时长出现断连的情况，非常影响用户体验，鉴于个人难以忍受这种操作体验，所以就四处寻找解决办法，这次运气不错，在[提高国内访问 GitHub 的速度的 9 种方案](https://blog.csdn.net/a1405/article/details/115438017)及[GitHub下载慢？可以试试下面的方法提升速度](https://www.secn.net/article/1562784.html)这两篇文章里，很容易就找到了。

<!-- more-->

平时使用的话，推荐使用hub.fastgit.org镜像源或者github.com.cnpmjs.org镜像源，这两个github镜像源的使用体验个人感觉很不错。

```
git clone https://github.com/XXXX/仓库名.git                               
```

使用方法也非常简单，将github.com替换成hub.fastgit.org即可

```
git clone  https://hub.fastgit.org/XXXX/仓库名.git
```

有时也会遇到将项目push到github远端速度慢的问题，这里也可以逆向思维，切换镜像源的方法，来提升上传速度。

最后这里在附上Segmentfault大佬民工哥的文章[三年 Git 使用心得 & 常见问题整理](https://segmentfault.com/a/1190000023734704)，希望可以帮到大家。

## OK！本期关于如何解决来自github的警告:Dependabot alerts就到此为止。喜欢的话请支持、转发、订阅！同时也欢迎各位大佬指出不足之处！在此本人万分感谢！