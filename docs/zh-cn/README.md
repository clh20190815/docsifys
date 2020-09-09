# 侧边栏

>  在index.html中开启配置 **loadSidebar**

~~~


<script>
  window.$docsify = {
    loadSidebar: true
  }
</script>
<script src="//cdn.jsdelivr.net/npm/docsify/lib/docsify.min.js"></script>
~~~

> 创建并编写_sidebar.md

~~~
<!-- docs/_sidebar.md -->
<!--[侧边栏标题](存放路径)-->
* [侧边栏](zh-cn/)

~~~

> 嵌套侧边栏

* 每个文件夹下都可以创建_sidebar.md,这样就可以让目录拥有自己的侧边栏
,当然你也可以配置不必要的回退过程 **alias**
~~~
<script>
  window.$docsify = {
    loadSidebar: true,
    alias: {
      '/.*/_sidebar.md': '/_sidebar.md'
    }
  }
</script>
~~~

 
