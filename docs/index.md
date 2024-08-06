# Vue 简介

Vue 是一款用于构建用户界面的 JavaScript 框架，它基于标准 HTML、CSS 和 JavaScript 构建，并提供了一套声明式的、组件化的编程模型，帮助你高效地开发用户界面。无论是简单还是复杂的界面，Vue 都可以胜任。


???+ example "简单示例"

    === "App.vue"

        ```ts linenums="1"
        import { createApp, ref } from 'vue'

        createApp({
        setup() {
            return {
            count: ref(0)
            }
        }
        }).mount('#app')
        ```
    
    === "main.html"

        ```html linenums="1"
        <div id="app">
          <button @click="count++">
            Count is: {{ count }}
          </button>
        </div>
        ```
  