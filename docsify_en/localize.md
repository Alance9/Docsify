<!-- 本地化 -->

> ### 1. File Localization

**Switch to the English sidebar and documents via the navigation bar**

> **Create a new localized catalog**

Create a new localization catalog, such as the English localization catalog docsify_en.

The first page under the general directory. Sidebar. Navigation bar. README. The main content and other MD documents are copied to the localization catalog for translation modification.

![本地化目录](../_media/_resources/本地化目录.png ':size=25%')


> **Localize the MD file**

GT4T translates and modifies files, and it is no problem to use third-party translation software to share files, but it is not recommended to use confidential documents.

![翻译文件1](../_media/_resources/翻译文件1.png ':size=30%')

![翻译文件2](../_media/_resources/翻译文件2.png ':size=50%')


> **From the project's navigation bar, switch to the localization sidebar and the corresponding document**

Set the paths to jump to the general directory respectively. README for subdirectories.

?> When switching to a subdirectory, it automatically obtains the sub-sidebar _sidebar under the directory, so as to realize the language switching.


```docsifyBlog/_navbar.md
<!-- Main Navigation Bar -->

* Language
  * [:uk: English](/docsify_en/README.md "English")
  * [:cn: 简体中文](/README.md "Chinese")

```


```docsifyBlog/docsify_en/_navbar.md
<!-- Subnavigation Bar -->

* Language
  * [:uk: English](/docsify_en/README.md "English")
  * [:cn: 简体中文](/README.md "Chinese")
```
![本地化1](../_media/_resources/本地化1.png ':size=100%')

![本地化2](../_media/_resources/本地化2.png ':size=100%')

> ### 2. Plugin Localization

**Switch to the Chinese and English language packs targeted by the $t() function via global variables**

IL8N plug-in address: https://github.com/woai3c/i18n-replace

il8n cannot be used for Docsify on its own, it requires Vue + il8n to be used together.

> Install the IL8N

 `npm i -g i18n-replace`

> Baidu Translate applies for universal text translation

```    
https://fanyi-api.baidu.com/product/11
Management Control Platform - Developer information，fetch APPID, Keys
1 million characters can be called for free every month.
```

> Copy modify i18n.config.js

?> Modify the translation, appid, key, entry (translation file path), to (Translation Language), mode, extra (file format)

Translation of .vue and .js files is supported by default, and other files such as extra: /(\.html)|(\.md)$/


``` js
// i18n.config.js

module.exports = {
    delay: 1500, // 自动翻译延时，必须大于 1000 ms，否则调用百度翻译 API 会失败
    mapFile: '', // 需要生成默认 map 的文件
    appid: '', // 百度翻译 appid
    key: '', // 百度翻译密钥
    output: 'i18n.data.js', // i18n 输出文件
    indent: 4, // i18n 输出文件缩进
    entry: '', // 要翻译的入口目录或文件，默认为命令行当前的 src 目录
    prefix: '', // i18n 变量前缀  i18n 变量生成规则 prefix + id + suffix
    suffix: '', // i18n 变量后缀
    id: 0, // i18n 自增变量 id
    translation: false, // 是否需要自动翻译中文
    to: 'en', // 中文翻译的目标语言
    mode: 1, // 0 翻译所有 i18n 数据，1 只翻译新数据
    loader: 'loader.js',
    pluginPrefix: '$t', // i18n 插件前缀 例如 vue-i18n: $t， react-i18next: t
    include: [], // 需要翻译的目录或文件
    exclude: [], // 不需要翻译的目录或文件 如果 exclude include 同时存在同样的目录或文件 则 exclude 优先级高
    extra: /(\.a)|(\.b)$/, // 默认支持 .vue 和 .js 文件 如果需要支持其他类型的文件，请用正则描述 例如这个示例额外支持 .a .b 文件
}
```

> Execute i18n.config.js

Execute the command `rep`


```
E:\Code\docsifyBlog> rep
docsifyBlog generates translated output files in the directory i18n.data.js
```

![本地化翻译](../_media/_resources/本地化翻译.png)

> Use it with Vue in the future


```
Create i18n instance，Mount to Vue instance，$t() the function is located in both Chinese and English
Define a global variable locale，use the button to switch between Chinese and English（zh. en）
```
