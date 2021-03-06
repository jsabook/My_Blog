---
title: 如何为自己的爱机神舟TX6-CT5DA加装固态硬盘
date: 2021-01-22 14:19:19
categories: [神舟战神TX6-CT5DA,固态硬盘]
tags: [神舟战神TX6-CT5DA,固态硬盘]
toc: true
copyright: true
---

在学习Linux系统的使用的过程中，在学习了一段时间之后，我觉得有必要为自己的战神（TX6-CT5DA）加装一块128G的固态硬盘用于安装ubuntu18.04系统，本文属于Ubuntu与ROS系列。

# 在本文中主要介绍我是如何为自己的爱机神舟TX6-CT5DA加装固态硬盘

<!-- more -->

## 使用场景

<font color=#999AAA >项目场景：如果你想使用Windows与Linux两种系统，比如Ubuntu之类的，同时你追求更高的性能，那么显然双系统可能是你更好的选择。</font>

### 前期准备

1.提前下载好自己需要的Linux安装镜像，比如Ubuntu16.04

2.准备一个大小至少为32G的U盘

3.准备一块不小于128G的固态硬盘，不建议机械硬盘，这里就不多解释了。

这里附上我所购买的[宏想固态](https://m.tb.cn/h.488QMNG?sm=429b6e)

4.准备必要的拆机工具，比如螺丝刀。

### 具体步骤

1.首先将笔记本电脑关机，如果是Win10家庭版可以使用快捷组合键Win+X，U，U即可快速关机。

2.取下笔记本的电池

3.将笔记本后盖的螺丝拧下来

4.使用专用的撬棒沿着后盖的纹路一点一点撬开，过程中要胆大心细，每撬开一处可以听到清脆的响声，注意过程中不要太过着急，卡扣比较脆弱，很容易弄断。

<font color=#999AAA >注意：不建议大力出奇迹的想法，出问题的看客责任自负，还有请小白同学慎重考虑是否要亲力亲为。</font>

{% asset_img 1.jpg This is an image %}

![](https://github.com/sujit-168/Blog-Picture/raw/master/My%20Blog/%E5%A6%82%E4%BD%95%E4%B8%BA%E8%87%AA%E5%B7%B1%E7%9A%84%E7%88%B1%E6%9C%BA%E7%A5%9E%E8%88%9FTX6-CT5DA%E5%8A%A0%E8%A3%85%E5%9B%BA%E6%80%81%E7%A1%AC%E7%9B%98/1.jpg)

这个是我拆机后的图片，神舟战神T系列可以看到，英特尔 i5 9400 CPU芯片并不是直接焊在主板上的，也就是说，之后有可能可以更换更高性能的CPU芯片，比如i5 10400，当然这还是需要考虑功耗与散热方面的影响。

![](https://github.com/sujit-168/Blog-Picture/raw/master/My%20Blog/%E5%A6%82%E4%BD%95%E4%B8%BA%E8%87%AA%E5%B7%B1%E7%9A%84%E7%88%B1%E6%9C%BA%E7%A5%9E%E8%88%9FTX6-CT5DA%E5%8A%A0%E8%A3%85%E5%9B%BA%E6%80%81%E7%A1%AC%E7%9B%98/2.jpg)

因为是蓝天公模，所以后盖也很有特点。

![](https://github.com/sujit-168/Blog-Picture/raw/master/My%20Blog/%E5%A6%82%E4%BD%95%E4%B8%BA%E8%87%AA%E5%B7%B1%E7%9A%84%E7%88%B1%E6%9C%BA%E7%A5%9E%E8%88%9FTX6-CT5DA%E5%8A%A0%E8%A3%85%E5%9B%BA%E6%80%81%E7%A1%AC%E7%9B%98/3.jpg)

这是加上固态硬盘后的图片，直接将其对应好接口插入即可

![](https://github.com/sujit-168/Blog-Picture/raw/master/My%20Blog/%E5%A6%82%E4%BD%95%E4%B8%BA%E8%87%AA%E5%B7%B1%E7%9A%84%E7%88%B1%E6%9C%BA%E7%A5%9E%E8%88%9FTX6-CT5DA%E5%8A%A0%E8%A3%85%E5%9B%BA%E6%80%81%E7%A1%AC%E7%9B%98/4.jpg)

可以看到，还有一个内存条接口和M.2固态硬盘接口

![](https://github.com/sujit-168/Blog-Picture/raw/master/My%20Blog/%E5%A6%82%E4%BD%95%E4%B8%BA%E8%87%AA%E5%B7%B1%E7%9A%84%E7%88%B1%E6%9C%BA%E7%A5%9E%E8%88%9FTX6-CT5DA%E5%8A%A0%E8%A3%85%E5%9B%BA%E6%80%81%E7%A1%AC%E7%9B%98/5.jpg)

难得自己拆机一次，建议备好清灰工具之类的，可以为自己的电脑清清灰。

![](https://github.com/sujit-168/Blog-Picture/raw/master/My%20Blog/%E5%A6%82%E4%BD%95%E4%B8%BA%E8%87%AA%E5%B7%B1%E7%9A%84%E7%88%B1%E6%9C%BA%E7%A5%9E%E8%88%9FTX6-CT5DA%E5%8A%A0%E8%A3%85%E5%9B%BA%E6%80%81%E7%A1%AC%E7%9B%98/6.jpg)

清灰完成后先不要着急合上后盖，先装上电池，开机检查新的固态硬盘能否正常进行读写操作。避免返工。

![](https://github.com/sujit-168/Blog-Picture/raw/master/My%20Blog/%E5%A6%82%E4%BD%95%E4%B8%BA%E8%87%AA%E5%B7%B1%E7%9A%84%E7%88%B1%E6%9C%BA%E7%A5%9E%E8%88%9FTX6-CT5DA%E5%8A%A0%E8%A3%85%E5%9B%BA%E6%80%81%E7%A1%AC%E7%9B%98/7.jpg)

检查完成后没有问题，先进行关机，因为不取下电池，无法安装后盖。

之后按照正常流程装回所有部分即可。

## OK！本期关于如何为自己的爱机神舟TX6-CT5DA加装固态硬盘就到此为止。喜欢的话请支持、转发、订阅！同时也欢迎各位大佬指出不足之处！在此本人万分感谢！

