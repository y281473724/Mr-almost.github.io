---
title: git备份博客
date: 2018-04-03 15:35:05
tags:
---
1.gitbash的位置定位到git指向username.github.io的文件夹，把博客代码放在这里
2.创建分支hexo，把博客的代码上传到这个分支
```
git branch hexo
git checkout hexo
git add .
git commit -m "blog"
git push origin hexo
```
3.在setting–Branches–Default branch中将backup设置为默认的分支，这样git push时就会push到这个分支上
4.对博客进行更新
```
依次执行git add . 、 git commit -m "some message" 、 git push推送源文件
执行hexo g -d 生成部署博客
```