<template>
    <div id="app">
        <nav-bar></nav-bar>
        <div id="main">
            <router-view></router-view>
        </div>
        <footer-bar></footer-bar>
    </div>
</template>

<script>
    import navBar from "./components/navBar.vue"
    import footerBar from "./components/footerBar.vue";
    export default {
        name: 'app',
        components: {
            navBar,
            footerBar
        }
    }
</script>

<style scoped>
    
    #main{
        min-height:100%;
        padding-bottom: 260px;
        background-image: url('assets/background.jpg');
        background-attachment:fixed; 
        background-size:cover;
        
    }
    
</style>
