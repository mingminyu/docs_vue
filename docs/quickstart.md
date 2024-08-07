# 快速上手

## 1. 线上尝试 Vue

想要快速体验 Vue，你可以直接试试 [Vue Playround](https://play.vuejs.org/)。如果你更喜欢不用任何构建的原始 HTML，可以使用 JSFiddle 入门。

如果你已经比较熟悉 Node.js 和构建工具等概念，还可以直接在浏览器中打开 StackBlitz 来尝试完整的构建设置。

## 2. 创建一个 Vue 应用

!!! note "前提条件"

    - 熟悉命令行
    - 已安装 18.3+ 的 Node.js

在本节中，我们将介绍如何在本地搭建 [Vue 单页应用](https://cn.vuejs.org/guide/extras/ways-of-using-vue.html#single-page-application-spa)。创建的项目将使用基于 Vite 的构建设置，并允许我们使用 Vue 的[单文件组件](https://cn.vuejs.org/guide/scaling-up/sfc.html) (SFC)。

确保你安装了最新版本的 Node.js，并且你的当前工作目录正是打算创建项目的目录。在命令行中运行以下命令 (不要带上 `$` 符号)：

???+ note "使用 Vite 创建项目"

    === "npm"

        ```bash
        npm create vue@latest
        ```

    === "pnpm"

        ```bash
        pnpm create vue@latest
        ```

    === "yarn"

        ```bash
        yarn create vue@latest
        ```

    === "bun"

        ```bash
        bun create vue@latest
        ```

这一指令将会安装并执行 `create-vue`，它是 Vue 官方的项目脚手架工具。你将会看到一些诸如 TypeScript 和测试支持之类的可选功能提示：

```bash
$ pnpm create vue@latest
Vue.js - The Progressive JavaScript Framework

✔ Project name: … hello_vue
✔ Add TypeScript? … No / Yes
✔ Add JSX Support? … No / Yes
✔ Add Vue Router for Single Page Application development? … No / Yes
✔ Add Pinia for state management? … No / Yes
✔ Add Vitest for Unit Testing? … No / Yes
✔ Add an End-to-End Testing Solution? › No
✔ Add ESLint for code quality? … No / Yes
✔ Add Vue DevTools 7 extension for debugging? (experimental) … No / Yes
```

如果不确定是否要开启某个功能，你可以直接按下回车键选择 No。在项目被创建后，通过以下步骤安装依赖并启动开发服务器：

???+ note "运行服务"

    === "npm"

        ```bash
        cd hello_vue
        npm install
        npm run dev
        ```

    === "pnpm"

        ```bash
        cd hello_vue
        pnpm install
        pnpm run dev
        ```

    === "yarn"

        ```bash
        cd hello_vue
        yarn install
        yarn dev
        ```

    === "bun"

        ```bash
        cd hello_vue
        bun install
        bun run dev
        ```

## 3. 通过 CDN 使用 Vue

