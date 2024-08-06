# Vue 简介

Vue 是一款用于构建用户界面的 JavaScript 框架，它基于标准 HTML、CSS 和 JavaScript 构建，并提供了一套声明式的、组件化的编程模型，帮助你高效地开发用户界面。无论是简单还是复杂的界面，Vue 都可以胜任。

???+ example "简单示例"

    === "组合式"

        ```ts linenums="1" hl_lines="4-8" title="App.vue"
        import { createApp, ref } from 'vue'

        createApp({
          setup() {
            return {
              count: ref(0)
            }
          }
        }).mount('#app')
        ```

        ```html linenums="1" title="main.html"
        <div id="app">
          <button @click="count++">
            Count is: {{ count }}
          </button>
        </div>
        ```
    
    === "选项式"

        ```ts linenums="1" hl_lines="4-8" title="App.vue"
        import { createApp } from 'vue'

        createApp({
          data() {
            return {
              count: 0
            }
          }
        }).mount('#app')
        ```

        ```html linenums="1" title="main.html"
        <div id="app">
          <button @click="count++">
            Count is: {{ count }}
          </button>
        </div>
        ```

上面的示例展示了 Vue 的两个核心功能：

- **声明式渲染**：Vue 基于标准 HTML 拓展了一套模板语法，使得我们可以声明式地描述最终输出的 HTML 和 JavaScript 状态之间的关系。
- **响应性**：Vue 会自动跟踪 JavaScript 状态，并在其发生变化时响应式地更新 DOM。


!!! tip "预备知识"

    文档接下来的内容会假设你对 HTML、CSS 和 JavaScript 已经基本熟悉。如果你对前端开发完全陌生，最好不要直接从一个框架开始进行入门学习——最好是掌握了基础知识再回到这里。如有需要，你可以通过这些 JavaScript、HTML 和 CSS 概述来检验你的知识水平。如果之前有其他框架的经验会很有帮助，但也不是必须的。

## 1. 渐进式框架

