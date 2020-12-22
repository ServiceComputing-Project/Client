<template>
    <div>
        <footer>
        <ul>
          <p @click="toHomePage" >My Blog</p>
          <li>
            <ul>
                <li><Icon type="logo-github" :size="25" style="margin-right: 5px"/><span style="font-size:20px;">Github</span></li>
                <li><a href="https://github.com/ServiceComputing-Project/Docs" target="_blank">Docs</a></li>
                <li><a href="https://github.com/ServiceComputing-Project/Client" target="_blank">FrontEnd</a></li>
                <li><a href="https://github.com/ServiceComputing-Project/Server" target="_blank">BackEnd</a></li>
            </ul>
            </li>
            <li>
            <ul>
                <li><Icon type="md-people" size="25" style="margin-right: 5px"/><span style="font-size:20px;">FrontEnd Team</span></li>
                <li><a href="https://github.com/zxy0616" target="_blank">zxy0616</a></li>
                <li><a href="https://github.com/zhangxy0" target="_blank">zhangxy0</a></li>
            </ul>
            </li>
            <li>
            <ul>
                <li><Icon type="ios-people" size="25" style="margin-right: 5px"/><span style="font-size:20px;">BackEnd Team</span></li>
                <li><a href="https://github.com/Annecle" target="_blank">Annecle</a></li>
                <li><a href="https://github.com/EmilyYoung9" target="_blank">EmilyYoung9</a></li>
                <li><a href="https://github.com/beikenken" target="_blank">beikenken</a></li>
                <li><a href="https://github.com/utaZ" target="_blank">utaz</a></li>
            </ul>
            </li>
            <router-link v-if="this.$route.name ==='home'" style="float:right; margin-right: 60px; font-size: 30px;color: black;" to="/signin">
                <Button >登录</Button>
            </router-link>
            <router-link v-else-if="this.$route.name ==='articleList'" style="float:right; margin-right: 60px; font-size: 30px;color: black;" to="/">
                <Button @click="signOut">退出</Button>
            </router-link>
          </ul>

        </footer>
    </div>
</template>

<script>
    export default {
        name: "footerBar",
        methods:{
            toHomePage(){
                if(window.localStorage.isLogin === '1')
                    this.$router.push('/articleList')
                else
                    this.$router.push('/')
            },
            expend(){
                let s = document.getElementById("search")
                s.style.width='400px'
                this.$Message.warning('未完成的功能，敬请期待!')
            },
            narrow(){
                let s = document.getElementById("search")
                s.style.width='250px'
            },
            signOut(){
                this.$store.commit('$_removeStorage')
            }
        }
    }
</script>

<style scoped>
    div{
        background-color: #AFEEEE;
        width: 12%;
        height: 100%;
        position:absolute;
        bottom:0;
        left:0
    }

    footer{
        display: flex;
        overflow: hidden;
        //padding: 20px;
        color: rgb(0, 0, 0);
        justify-content: space-around;
    }

    footer ul{
        list-style-type: none;
        margin: 0;
        padding: 0;
        width: 200px;
    }

    footer ul li{
        display: block;
        padding: 8px 16px;
        text-decoration: none;
    }

    footer li:first-child{
        margin: 0px;
    }

    a{
        color: rgb(0, 0, 0);
        font-size:15px;
    }
    p {
    	margin-left:0px;
        font-size: 30px;
        letter-spacing: 3px;
        text-transform: uppercase;
        font-family: sans-serif;
        color: rgb(0, 0, 0);
        font-weight: bold;
        
    }
    Button{
    	font-size: 25px;
    	color: black;
    	background-color: #AFEEEE;
    	border:1px solid black;
    	
    }
</style>
