---
title: Hello Vue
date: 2023-02-07 00:29:20
tags: Vue 起手式：Vue select option
---
        //寫法1：等有需要時再mount到某節點上
        const vm = Vue.createApp({
            data() {
                return {
                    message: ""
                }
            }
        })
        vm.mount("#app");

        // 寫法2
        const vm = {
            data() {
                return {
                    message: ""
                }
            }
        }
        Vue.createApp(vm).mount("#app");

        // 寫法3
        Vue.createApp({
            data(){
                return {
                    message:""
                }
            }
        }).mount("#app");

        // 寫法4:js物件是傳址特性，透過...淺拷貝
        const dataObj = {
            message: ""
        }
        const vm = Vue.createApp({
            data() {
                return {...dataObj}
            }
        })
        vm.mount("#app");

[Github](https://github.com/bonnieli1414/Vue_notion/blob/main/01.Vue_option.html)
