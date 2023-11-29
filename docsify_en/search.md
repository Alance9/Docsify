<!-- 搜索栏 -->

> ### Reference the Search Plug-in


```index.html
<script>
    window.$docsify = {
        // Custom search
        search: {
          maxAge: 86400000, // Expiration time in milliseconds, default one day
          placeholder: 'Type to search',

          // Support localization
          placeholder: {
            '/docsify_en/': 'Type to search',
            '/': '搜索'
          },

          noData: 'No Results!',

          // Support localization
          noData: {
            '/docsify_en/': 'No Results',
            '/': '找不到结果'
          },

          // The maximum level of the search title, 1 - 6
          depth: 6,
        }
    }
 </script>

<!-- Search -->
<script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/search.min.js"></script>
```

![搜索1](../_media/_resources/搜索1.png ':size=70%')

![搜索2](../_media/_resources/搜索2.png ':size=70%')