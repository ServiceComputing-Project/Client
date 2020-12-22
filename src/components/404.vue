<template>
    <div>
        <h1>ERROR!</h1>
        <p>Please check the URL,</br>or click the button 
        <router-link to="/"><Button >返回主页</Button></router-link></p>
    </div>
</template>

<script>
export default {
    name: 'errorPage'
}
</script>

<style scoped>
    div{
        text-align: center;
    }
    h1{
        padding-top: 100px;
        font-size: 40px;
    }
    p{
        margin: 20px 0;
        font-size: 25px;
    }
    Button{
    	font-size: 25px;
    }
</style>
