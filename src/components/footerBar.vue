<template>
    <div>
        <footer>
        <ul>
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
        //width: 100%;
        width: 12%;
        height: 93%;
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
        //margin-left: 10px;
        //margin-top: 5px;
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
</style>
