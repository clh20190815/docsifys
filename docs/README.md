# 快速开始

## 安装 docsify-cli
 
 ~~~
 npm i docsify-cli -g
 ~~~
  
## 初始化项目
 >如果想在项目的 ./docs 目录里写文档，直接通过 init 初始化项目。
 ~~~
 docsify init ./docs
 ~~~

## 开始写文档 

>初始化成功后，可以看到 ./docs 目录下创建的几个文件

* index.html 入口文件
* README.md 会做为主页内容渲染
* .nojekyll 用于阻止 GitHub Pages 忽略掉下划线开头的文件

直接编辑  **docs/README.md** 就能更新文档内容



## 本地预览
~~~
 docsify serve docs
~~~
