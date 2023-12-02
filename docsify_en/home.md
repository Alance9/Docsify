<!-- 封面 -->

***Cover _coverpage settings***

> ### 1. Cover Settings

```index.html
window.$docsify = {
    // enable rendering cover
    coverpage: true
}
```

`_coverpage.md` Defines the content of the homepage, which can replace the custom cover, and defaults to a random gradient.

?> Cover Default File Name _coverpage


```docsifyBlog/_coverpage.md
<!-- 首页 -->

# Alance <small>share v1.1.0</small>

- 分享编程与测试的经验

# Docsify 使用教程

<!-- [GitHub](https://github.com/docsifyjs/docsify/) -->
[Start Browse →](./README.md)

<!-- 替换封面 -->
![bg](_media/云朵与羊群-新1.png)

<!-- 设置背景色 -->
![color](#f0f0f0)
```

> ### 2. Cover Transparency Settings


```docsifyBlog/_plugins/style.css
section.cover.has-mask .mask{
    opacity:.1;
}
```

> ### 3. Homepage Introduction

 `[Start Browse →](/README)`, the cover jumps to the homepage introduction.

?> Home page introduces the default file name README


```docsifyBlog//README.md
## 🌻 快速搭建一个博客系统

> Docsify 框架搭建一个轻量化静态网站

> 可应用于，博客系统、个人简历、产品说明书、攻略指南 

> 像搭积木一样，利用多样可选的插件，快速搭建充满个性化的博客

🐹 遵循拿来主义，尊重前人的智慧，能用现成轮子，绝不手写 ![Parrot Shake](../_media/_resources/parrot.gif ':size=30×30')

```
![主页介绍](../_media/_resources/主页介绍.png ':size=870')