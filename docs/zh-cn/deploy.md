# 部署
## GitHub Pages
GitHub Pages 支持从三个地方读取文件
* docs/ 目录
* master 分支
* gh-pages 分支

我们推荐直接将文档放在 docs/ 目录下，在设置页面开启 GitHub Pages 功能并选择 master branch /docs folder 选项。


!> 可以将文档放在根目录下，然后选择 master 分支 作为文档目录。你需要在部署位置下放一个 .nojekyll 文件（比如 /docs 目录或者 gh-pages 分支）

## VPS

和部署所有静态网站一样，只需将服务器的访问根目录设定为 index.html 文件。

例如 nginx 的配置

~~~
server {
  listen 80;
  server_name  your.domain.com;

  location / {
    alias /path/to/dir/of/docs/;
    index index.html;
  }
}
~~~