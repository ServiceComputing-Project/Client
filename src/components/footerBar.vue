<template>
    <div>
        <footer>
            <ul>
                <li><Icon type="logo-github" :size="25" style="margin-right: 5px"/><span>Github</span></li>
                <li><a href="https://github.com/ServiceComputing-Project/Docs" target="_blank">Docs</a></li>
                <li><a href="https://github.com/ServiceComputing-Project/Client" target="_blank">FrontEnd</a></li>
                <li><a href="https://github.com/ServiceComputing-Project/Server" target="_blank">BackEnd</a></li>
            </ul>
            <ul>
                <li><Icon type="md-people" size="25" style="margin-right: 5px"/><span>FrontEnd Team</span></li>
                <li><a href="https://github.com/zxy0616" target="_blank">Zhang Xuanyu</a></li>
                <li><a href="https://github.com/xutaiqi" target="_blank">Zhang Xinyue</a></li>
            </ul>
            <ul>
                <li><Icon type="ios-people" size="25" style="margin-right: 5px"/><span>BackEnd Team</span></li>
                <li><a href="https://github.com/IYreality" target="_blank">Zhou Yuan</a></li>
                <li><a href="https://github.com/LeoBarwoo" target="_blank">Yang Ling</a></li>
                <li><a href="https://github.com/beikenken" target="_blank">Zhang Youfang</a></li>
                <li><a href="https://github.com/utaZ" target="_blank">Zou Wenrui</a></li>
            </ul>
            <ul>
                <li><Icon type="md-chatboxes" size="25" style="margin-right: 5px"/><span>Contact Us</span></li>
                <li><a><Icon type="logo-twitter" style="margin-right: 5px"/>Twitter</a></li>
                <li><a><Icon type="logo-facebook" style="margin-right: 5px"/>Facebook</a></li>
                <li><a><Icon type="logo-google" style="margin-right: 5px"/>Google</a></li>
            </ul>
        </footer>
    </div>
</template>

<script>
    export default {
        name: "footerBar"
    }
</script>

<style scoped>
    div{
        background-color: #AFEEEE;
        width: 100%;
        position:absolute;
        bottom:0;
    }

    footer{
        display: flex;
        overflow: hidden;
        padding: 20px;
        color: rgb(0, 0, 0);
        justify-content: space-around;
    }

    footer ul{
        list-style:none;
    }

    footer ul li{
        margin-left: 10px;
        margin-top: 5px;
    }

    footer li:first-child{
        margin: 0px;
    }

    a{
        color: rgb(0, 0, 0);
    }
</style>
