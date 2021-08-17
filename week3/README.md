# Week3 待辦清單 (Options API)
## 學習要點
1. 鍵盤修飾符 - `@keyup.enter="event"`
2. 修飾掉首尾的空白 `v-model.trim`
3. 阻擋元素的預設行為 `@click.prevent`
4. 樣式綁定 `:class`
5. 屬性綁定 `:id、:for、:checked`
6. 監聽變更事件 `@change`
7. 註冊一個局部指令 v-focus (這個指令只能在該實例中使用)，該指令功能是在頁面加載時，元素獲得焦點
    ```jsx
    <div id="app">
        <input type="text" v-focus>
    </div>

    <script>
    	Vue.creatApp({
    		directives: {
            focus: {
                mounted(el) {
                    el.focus()
                }
            }
        }
    	}).mount('#app');
    </script>
    ```