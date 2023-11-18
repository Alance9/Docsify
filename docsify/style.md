
> ###  1、自定义封面

`_coverpage.md` 定义首页内容，可替换自定义封面，默认为随机渐变

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

> ###  2、自定义主题色

`themeColor` 默认主题色为 `#42b983`

```index.html
window.$docsify = {
    // 主题色
    themeColor: "#96b97d"
}
```

> ###  3、其他设置

```index.html
window.$docsify = {
    // 目录标题
    name: 'Docsify 说明书',

    // 自定义目录级别
    subMaxLevel: 3,
    
    // 加载左侧目录
    loadSidebar: true,

    // 避免不必要的回退
    alias: {
    '/.*/_sidebar.md': '/_sidebar.md'
    },

    // 加载顶部导航栏
    loadNavbar: true,

    // 开启渲染封面
    coverpage: true,

    // 只在访问主页时加载封面
    onlyCover: false
}
```