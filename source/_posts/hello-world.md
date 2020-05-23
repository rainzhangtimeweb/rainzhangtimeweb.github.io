title: Hexo 相关命令
tags: []
categories:
  - 技术
  - hexo
date: 2020-05-13 16:10:28
---
官网: https://hexo.io/

## 快速开始

### 新建一篇文章

``` bash
$ hexo new "My New Post"
```

更多信息: [新建文章](https://hexo.io/docs/writing.html)

### 启动hexo服务

``` bash
$ hexo server
```

更多信息: [启动服务](https://hexo.io/docs/server.html)

### 创建静态文件

``` bash
$ hexo generate
```

更多信息: [生成静态文件](https://hexo.io/docs/generating.html)

### 发布文章

``` bash
$ hexo deploy
```

更多信息: [发布](https://hexo.io/docs/one-command-deployment.html)

### 启动边预览边编辑
#### Hexo Admin
cd 在Hexo网站目录下,安装Hexo Admin插件
``` bash
$ npm install --save hexo-admin
```
#### 启动本地服务器并打开管理界面
``` bash
$ hexo server -d
$ open http://localhost:4000/admin
```

#### 启动本地服务器并打开管理界面
添加搜索插件
``` bash
npm install hexo-generator-searchdb --save
```
blog下的_config.yml文件，进行编辑
``` bash
search:
    path: search.xml
    field: post
    format: html
    limit: 10000
```
修改主题配置文件,/blog/themes/next下的_config.yml文件
``` bash
local_search:
    enable: true
```