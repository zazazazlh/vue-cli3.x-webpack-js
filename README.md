# vue-cli3.x-webpack-js

## Project setup

```
npm install
```

### Compiles and hot-reloads for development

```
npm run serve
```

### Compiles and minifies for production

```
npm run build
```

### Lints and fixes files

```
npm run lint
```

### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/).


### 目录结构
# cli 3.x
├── 'node_modules'     // npm下载包都在这个文件夹
├── 'public'
│   ├── 'favicon.ico'
│   └── 'index.html'  // 作为入口模板,最后打包文件所在地，也是main,js 绑定的 dom
├── 'src'             // 整个工程文件目录
│   ├── 'api'         // 创建用来管理接口的文件夹
│   │   └── 'index.js'    // axios 入口使用
│   ├── 'assets'      // 静态资源管理负责管理图片文字一类的
│   │   ├── 'font'    // 存放字体库文件夹
│   │   └── 'img'     // 存放图片的文件夹
│   ├── 'components'  // 存放组件文件夹
│   │   └── 'HelloWorld.vue'     // 这是一个名叫HelloWorld.vue组件
│   ├── 'config'      // 项目配置的文件夹
│   │   └──  'index.js'          // 利用node 找包特性 起名index.js 可以快速导包
│   ├── 'directive'   // 自定义指令文件夹
│   │   └── 'index.js'           // 利用node 找包特性 起名index.js 可以快速导包
│   ├── 'lib'         //工具包
│   │   ├── 'tools.js'           // 存放和业务无关工具性质的js代码
│   │   └── 'util.js'            //存放和业务相关工具性质的js代码
│   │   └── 'axios.js'            //ajax 异步封装
│   ├── 'mock'        // 模拟返回数据文件夹
│   │   └── 'index.js'           // 利用node 找包特性 起名index.js 可以快速导包
│   ├── 'router'      // 路由相关
│   │   ├── 'index.js'            // 利用node 找包特性 起名index.js 可以快速导包
│   │   └── 'router.js'           // 路由配置
│   ├── 'store'        // Vuex状态管理文件夹
│   │   ├── 'plugin'   // Vuex配置文件夹
│   │   │   └── 'saveInLocal.js'         // vuex 文件内容本地化储存
│   │   ├── 'module'   // 提取的特定模块的文件夹
│   │   │   └── 'user.js'         // 保存user模块的vuex js
│   │   ├── 'actions.js'          // 提取出vuex actions模块
│   │   ├── 'index.js'            // 利用node 找包特性 起名index.js 可以快速导包
│   │   ├── 'mutations.js'        // 提取出vuex mutations模块
│   │   ├── 'getters.js'          // 提取出vuex getters模块
│   │   └── 'state.js'            // 提取出vuex state模块
│   ├── 'views'        // 视图组件 和 公共组件
│   │   ├── 'About.vue'
│   │   └── 'Home.vue'
│   ├── App.vue     // 由于render 特性 所以需要一个被渲染的vue文件
│   ├── main.js     // 项目入口，文件打包会找这个文件，并且将这个文件的内容打包
├── .browserslistrc      //目标浏览器配置表
├── .editorconfig        // 编辑器配置 -额外添加
├── .env.development     // 环境变量-开发 -额外添加
├── .env.production      // 环境变量-生产 -额外添加
├── .gitignore           // 忽略用git提交省略的提交目录
├── babel.config.js      //  高级语法转低级语法
├── package.json
├── package-lock.json    // 锁版本包
├── postcss.config.js    //CSS预处理器 -额外添加
├── README.md
└── vue.config.js        // 项目自定义配置
