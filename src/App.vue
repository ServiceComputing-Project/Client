<template>
    <div id="app">
        <footer-bar></footer-bar>
        <router-view></router-view>
    </div>
</template>

<script>
    import footerBar from "./components/footerBar.vue";
    export default {
        name: 'app',
        components: {
            footerBar
        }
    }
</script>

<style scoped>
    #app{
        background-image: url('assets/background.jpg');
        background-attachment:scroll; 
        background-size:cover;        
    }
</style>
