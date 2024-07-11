## pnpm monorepo+vue3+vite 搭建组件库并发布到私有仓库

##目录结构描述
```
.
├── README.md
├── example // 引入组件库的使用示例
├── packages
│   └── components
│       ├── index.html
│       ├── index.js // 集中导出所有组件
│       ├── package.json // 声明要发布的组件库信息
│       ├── src
│       │   ├── App.vue
│       │   ├── button // 组件库组件
│       │   │   ├── index.js // 用于导出button组件
│       │   │   └── src
│       │   │       └── index.vue // 组件代码
│       │   ├── index.js // 集中导出src下的所有组件
│       │   ├── main.js
│       │   ├── style.css
│       │   └── utils
│       │       └── withInstall.js // 导出组件的方法
│       └── vite.config.js
├── pnpm-workspace.yaml
├── package.json
```