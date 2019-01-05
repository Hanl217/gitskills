# Git技巧复习
 
## Git简介  
Git：分布式版本控制系统  
CVS、SVN：集中式版本控制系统，需要联网而且速度慢
 
## 安装Git  
Windows 直接从官网下载安装  
Git Blash:  
  `$ git config --global user.name "Your Name"`  
  `$ git config --global user.email "email@example.com"`  
(--global 机器上所有的Git仓库)
 
## 版本库(repository)  
本质就是Git管理的一个目录  
1 创建目录  
`$ mkdir filename`  
`$ cd filename`  
`$ pwd`显示当前目录  
2 目录-->仓库  
`$ git init`空仓库；.git用来跟踪管理版本库  
`$ ls -ah`显示隐藏目录
 
所有的版本控制器只能跟踪文本文件的改动，比如txt，网页，代码等，  
而图片、视频以及Word等二进制文件无法跟踪具体改动  
**文本编码：UTF-8（推荐）**  
Windows自带记事本开头添加了0xefbbbf（十六进制），导致它不适用于编辑UTF-8文件  
--> **Notepad++**（编码设置：UTF-8 without BOM）
 
1 文件添加到仓库  
`$ git add <file>`可以多次add不同文件  
2 文件提交到仓库  
`$ git commit -m <message>`一次commit所有文件
 
 ## 时光机穿梭
