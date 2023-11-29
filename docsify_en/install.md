<!-- Getting Started -->

> ###  1. Install the Node. JS.

Docsify relies on node.js, Download and Install: https://nodejs.org/en


```
Environment Variables
NODE_PATH ：D:\NodeJs\node_modules

User Variable
D:\NodeJs\node_global

The installation is complete
C:\Users\Z>node -v
v18.17.0

C:\Users\Z>npm -v
9.6.7
```

> ### 2. Install Docsify

Check all permissions under the NodeJs installation directory (security-full control), run CMD as an administrator, and install globally.


```
npm i docsify-cli -g
```

> ### 3. Initialize Docsify

Initialize and create the docs directory and default files.

-  `index.html` Entry file
-  `README.md` Home page content
-  `.nojekyll` Prevent GitHub Pages from ignoring files that begin with an underscore


```
docsify init docs

Initialization succeeded! Please run docsify serve docs
```

> ### 4. Run Docsify

 `docsify serve ` Start the local server with hot reload to debug


```
docsify serve docs

Serving C:\Users\Z\docs now.
Listening at http://localhost:3000
```

![启动页面](../_media/_resources/index.png ':size=70%')