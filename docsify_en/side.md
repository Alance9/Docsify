<!-- 侧边栏 -->

***The edited document requires access to the entrance, which is the sidebar menu _sidebar.***

> ### 1. Sidebar Settings


```index.html
window.$docsify = {
    // custom directory level
    subMaxLevel: 3,
    // load the sidebar
    loadSidebar: true,
}
```

?> The sidebar default file name is _sidebar.md


```docsifyBlog/_sidebar.md 
* Getting started with Dosify

    * [Getting started](docsify_en/install)
```

> ### 2. Multiple sidebars

If there are multiple sidebars, the main sidebar is taken by default.

If there is a child sidebar, the child sidebar is taken, and if there is no child sidebar, the main sidebar is taken.

?> When switching to a subdirectory, it automatically obtains the sub-sidebar _sidebar under the directory, so as to achieve localization and specific viewing [Localizaction](/docsify/localize)


```docsifyBlog/_sidebar.md
<!-- Main Sidebar -->

* 🌻 快速搭建一个博客系统

* Dosify 入门

    * [入门](docsify/install)
    * [项目架构](docsify/structure)
    * [主文件](docsify/pages)
    * [侧边栏](docsify/side)
    * [导航栏](docsify/nav)
    * [搜索框](docsify/search)
    * [本地化](docsify/localize)
    * [远程部署](docsify/deploy)
    * [常用插件](docsify/plugins)
    * [表情符号](docsify/emo)
    * [自定义设置](docsify/style)

```


```docsifyBlog/docsify_en/_sidebar.md
<!-- Sub Sidebar -->

* 🌻 Quickly build a blog system

* Getting started with Dosify

    * [Getting started](docsify_en_en/install)
    * [Project structure](docsify_en/structure)
    * [Home Page Document](docsify_en_en/style)
    * [Sidebar](docsify_en/side)
    * [Navigation Bar](docsify_en/nav)
    * [Search](docsify_en/search)
    * [Localization](docsify_en/localize)
    * [Remote Deploy](docsify_en/deploy)
    * [Common plug-ins](docsify_en/plugins)
    * [emoji](docsify_en/emo)
    * [Custom setting](docsify_en/style)
```