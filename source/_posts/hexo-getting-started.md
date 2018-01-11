---
title: Github+Hexo基础环境（for Mac）
date: 2018-01-11 12:36:37
categories: Tutorial
tags: Hexo
---
# 1、安装Hexo
```
brew install node
npm install -g hexo
```

# 2、生成本地静态页
```
mkdir blog && cd blog
hexo init
hexo generate   (或 hexo g)
hexo server（或 hexo s）
```

# 3、Github远程部署
## 3.1 配置_config.yml文件
```
deploy:
  type: git
  repo: https://github.com/[your_account]/[your_accout].github.io.git
  branch: master
```

## 3.2 安装git插件
```
npm install hexo-deployer-git --save
```

## 3.3 执行部署
```
hexo deploy（或 hexo d）
```

# 4、更多参考文章
http://ijiaober.github.io/2014/08/05/hexo/hexo-04/
https://thief.one/2017/03/03/Hexo%E6%90%AD%E5%BB%BA%E5%8D%9A%E5%AE%A2%E6%95%99%E7%A8%8B/
http://blog.csdn.net/bigpudding24/article/details/48196939

