<!-- 自定义设置 -->

> ###  1. Customize the Cover

 `_coverpage.md` Define the content of the homepage, which can replace the custom cover, and the default is a random gradient.


```_coverpage.md 
<!-- 首页 -->

# Alance <small>share 1.0</small>

> 分享编程与测试的经验

- HTML. CSS. JS
- PYTHON. JAVA. RUBY
- TEST FUNCTION. AUTO. API et

[Start Browse →](README.md)

<!-- 替换封面 -->
![bg](_media/云朵与羊群-新1.png)

```

> Cover transparency settings


```style.css
section.cover.has-mask .mask{
    opacity:.1;
}
```

> ###  2. Customize the Accent Color

 `themeColor` The default accent color is `#42b983`


```index.html
window.$docsify = {
    // theme color
    themeColor: "#96b97d"
}
```

> ###  3. Other Settings


```index.html
window.$docsify = {
    // title of the catalog
    name: 'Docsify',

    // custom Catalog Level
    subMaxLevel: 3,
    
    // load sidebar
    loadSidebar: true,

    // load the top navigation bar
    loadNavbar: true,

    // enable rendering cover
    coverpage: true,
}
```


```style.css
<!-- customize the style -->

nav {
    font: 16px bold;
}

nav.app-nav li {
    min-width: 30px;
    margin-right: 20px;
}

nav.app-nav li ul {
    min-width: 100px;
}

nav.app-nav a {
    color: #34495e;
}

nav.app-nav a.active {
    color: #34495e;
    border-bottom: none;
}

aside {
    margin-left: 30px;
}

aside .sidebar-nav ul li p{
    color: #96b97d;
}

aside .sidebar-nav ul li a {
    padding: 0;
}

section.cover.has-mask .mask{
    opacity:.1;
}
```
