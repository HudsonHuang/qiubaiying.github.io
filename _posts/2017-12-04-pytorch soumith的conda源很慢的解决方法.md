---
layout:     post
title:      pytorch soumith的conda源很慢的解决方法
date:       2017-12-04
author:     HudsonHuang
header-img: img/post-bg-debug.png
---

> pytorch soumith的conda源很慢的解决方法

那个清华镜像的版本又太低，尝试了很多办法，最终方案却很简单：
尝试用官网的pip源安装，如下：


```
pip install http://download.pytorch.org/whl/cu80/torch-0.2.0.post3-cp35-cp35m-manylinux1_x86_64.whl 
pip install torchvision
```

还是很慢的话，可以科学上网然后先把这个whl文件下载好后本地pip安装

```
pip install C:\Users\TT\Desktop\torch-0.2.0.post3-cp35-cp35m-manylinux1_x86_64.whl
```