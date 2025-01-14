---
title: 使用PE盘重装 Windows
date: 2022-1-4
description: 记得备份好资料
categories:
  - 教程
tags:
  - 系统
---

**重装系统**是我们较为常见的一种解决问题的方式

## 制作pe盘

### 准备工具

U盘（最好大于等于32G，因为之后需要装一些镜像，如果只是重装8G也足够了）

制作软件（此处使用WinPE，注意2.2之前版本的WinPE内核识别不了搭载十一代cpu机器的硬盘，所以最好用2.2及以上的版本）

### 开始制作

确保u盘在制作的时候***无重要资料留存***，并将之格式化

打开软件，在右下角*其它安装方式* 的位置选择**安装pe到u盘**，安装方法默认，待写入U盘选择你的U盘，单击立即安装到U盘即可

### 准备镜像

镜像可以去

[MSDN, 我告诉你 - 做一个安静的工具站 (itellyou.cn)](https://msdn.itellyou.cn/)

[NEXT, ITELLYOU](https://next.itellyou.cn/)

进行下载。找到所需的镜像，复制镜像的ed2k链接，使用迅雷或者其他的下载器下载镜像

下载完毕后，找到镜像的下载位置，将其复制到制作好的pe盘中。至此，准备工作完成

## 重装系统

接下来是重头戏

### 进入BIOS

重装系统之前需要把制作好的pe盘插入电脑的USB接口，按下电脑的开机键，在机器品牌logo出现时按下打开BIOS的对应键位（不同品牌的机器对应键位不同，可以百度搜索）

进入BIOS后找到调整硬盘启动顺序的功能区，将pe盘的启动顺序调整至最上层，然后保存退出即可。如此便可进入pe系统

### 格式化系统盘

进入pe系统后打开桌面上的diskgenius操作磁盘

* 此处需要将电脑的C盘格式化，务必**谨慎考虑后**操作，格式化之前务必做好**重要资料的备份和转移**
* 另外注意DiskGenius中显示的C盘**不一定**是机器的系统盘，可根据磁盘大小进行辨认，以防因为盘符不同造成资料丢失

确认无误后，可在DiskGenius中对机器的系统盘格式化

### 重装

格式化完成之后，退出DiskGenius，打开Windows系统安装器，依次选择系统盘、引导位置、镜像文件，在软件无报错的情况下无脑下一步。等待读条完毕后，机器重启，此时可***拔出U盘或者再次进入BIOS调整机器的硬盘启动顺序，否则将再次进入pe系统***

### 等待

机器重启后，会进入重装系统的下一个阶段，此时等待，直至小娜的提示音出现。（***如果在公共场所，务必提前关闭声音，避免社死***）

接下来进行win系统的一系列设置，建议跳过联网以加快进度

### 激活

按照界面的简单提示对系统进行一些设置，之后便可顺利进入Windows桌面。到这里系统重装基本完成

最后需要对新装的系统进行激活

入梦工具箱：[提取码:ark3](https://www.123pan.com/s/s928Vv-mliWd )
若链接失效请联系E管家公众号 2985586863（QQ），E管家提供免费的重装服务

