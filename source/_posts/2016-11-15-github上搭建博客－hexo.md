---
title: github上搭建博客－hexo
date: 2016-11-15 14:04:42
tags:
categories:
- web
---

1.
bloghexo    ／／建bloghexo文件夹
github 上创建lixuequn.github.io 仓库
2.
nvm install stable   //安装node
sudo npm install -g hexo  //bloghexo文件夹下面安装Hexo
hexo init   ／／bloghexo文件夹下面,初始化hexo
3.
hexo generate   //部署
4.
vim _config.yml   ／／修改配置文件，如下：
／／／／／／／／／／／／／／／／／／／／／／／／／／／／／／／／／
deploy:

     type:  git

     repo:  https://github.com/lixuequn/lixuequn.github.io.git
     branch:  master

／／／／／／／／／／／／／／／／／／／／／／／／／／／／／／／／／／

5.
 npm install hexo-deployer-git --save
6.
 hexo deploy     ／／提交



7.
添加标签
hexo new page "tags"
确认站点配置文件里有tag_dir: tags
确认主题配置文件里有tags: /tags
编辑站点的source/tags/index.md，添加
#---
title: tags
date: 2016-11-15 10:45:16
type: "tags"
comments: false
#---

添加分类
hexo new page "categories"
确认站点配置文件里有category_dir: categories
确认主题配置文件里有categories: /categories
编辑站点的source/categories/index.md，添加
#---
title: categories
date: 2015-10-20 06:49:50
type: "categories"
comments: false
#---
8.
##打赏
reward_comment: 坚持原创技术分享，您的支持将鼓励我继续创作！
wechatpay: /images/wx.png
alipay: /images/zfb.png

