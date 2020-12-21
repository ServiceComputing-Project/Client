<template>
    <div>
        <h1 style="font-family:Serif;font-weight:bold;">{{ helloMessage }}</h1>
     <!---   
        <ul>
            <li>API design: Swagger</li>
            <li>Back-end: Golang</li>
            <li>Front-end: Vue.js</li>
        </ul>
-->
        <p style="margin-top: 300px;font-size:25px;">Click the sign-in button to enjoy.</p>
        <p style="font-size:25px;">See more details in <a href="https://github.com/ServiceComputing-Project" target="_blank">Github</a></p>
    </div>
</template>

<script>

import axios from 'axios'

export default {
    name:'home',
    data(){
        return {
            helloMessage: 'WELCOME TO MY BLOG',
            articles: []
        }
    },
    created(){
        if(window.localStorage.isLogin === '1')
            this.$router.push('/articleList')
    },
    methods:{

    }
}
</script>

<style scoped>
    div{
        text-align: center;
    }

    h1{
        //margin-top: 100px;
        letter-spacing: 5px;
        font-size: 50px;
    }

    ul{
        margin-top: 30px;
        line-height: 30px;
    }
</style>
