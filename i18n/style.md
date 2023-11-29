<!-- 自定义设置 -->

>{` ###  1、${this.$t('0')}`}

`_coverpage.md{` 定义首页内容，可替换自定义封面，默认为随机渐`}

```_coverpage.md 
<!-- 首页 -->

# Alance <small>share 1.0</small>

>{` ${this.$t('2')}`}

- HTML. CSS. JS
- PYTHON. JAVA. RUBY
- TEST FUNCTION. AUTO. API et

[Start Browse →](README.md)

<!-- 替换封面 -->
![bg](_media/this.$t('3').png)

```

>{` ###  2、${this.$t('4')}`}

`themeColor{` ${this.$t('5')} `}#42b983`

```index.html
window.$docsify = {
    // 主题色
    themeColor: "#96b97d"
}
```

>{` ###  3、${this.$t('6')}`}

```index.html
window.$docsify = {
    // 目录标题
    name: {`Docsify ${this.$t('7')}`},

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

