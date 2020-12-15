# 说明
本文档使用*Mkdocs*构建。更多内容详见：[mkdocs.org](https://www.mkdocs.org)。

## Mkdocs 常用命令

* `mkdocs new [dir-name]` 创建一个新的文档工程
* `mkdocs serve`命令可以启动内建服务器，执行成功后，在浏览器打开[http://127.0.0.1:8000/](http://127.0.0.1:8000/) 即可预览。
* `mkdocs build` 将文档以网页形式构建到`site\`文件夹下
* `mkdocs -h` 输出帮助信息

## Mkdocs 目录结构

`apple-docs`文件夹中每个文件的作用：   

* `mkdocs.yml`此为配置文件，文档的结构、主题都可以在此设置。  
* `docs文件夹`撰写的 Markdown 文档都放在这个文件夹内。   
* `index.md`默认首页。  

## Mkdocs 主题

`MkDocs`项目托管在 github 上，在项目的`community wiki`中，提供了大量的[第三方主题](https://github.com/mkdocs/mkdocs/wiki/MkDocs-Themes)。
###  mkdocs-material
`mkdocs-material`可定制、可搜索、移动友好、支持40多种语言的翻译
#### mkdocs-material的安装和使用
```shell
pip install mkdocs-material
```

在`mkdocs.yml`中配置：

```
theme:
    name: material
```


### rtd-dropdown
名称为`rtd-dropdown`的主题非常好用，是内置主题 readthedocs 的升级版，相比于之前的版本，升级版的主题有以下几个优点：

* 支持菜单目录折叠。点击`+`可以展开，展开后会显示下一级的所有标题，如果还有下一级标题中还有子标题，则会嵌套显示`+`。
  
* `rtd-dropdown`主题取消了子目录的缩进，防止目录级别过多而导致排版出现问题。
  
* 对应的`markdown`文档只存在一个一级标题的情况下，将不予显示在导航目录中。

然而，某些时候展开目录时，`+`会覆盖文字，不美观。

#### rtd-dropdown的安装和使用
```shell
 pip install mkdocs-rtd-dropdown
```

在`mkdocs.yml`中配置：

```
theme: rtd-dropdown
```
