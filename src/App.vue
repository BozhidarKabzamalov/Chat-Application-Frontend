<template>
    <div id="app">
        <router-view/>
    </div>
</template>

<script>
export default {
    mounted(){
        this.$store.dispatch('autoLogin');
    }
}
</script>

<style>
@import "../node_modules/@fortawesome/fontawesome-free/css/all.css";

*, *:after, *:before {
    margin: 0;
    padding: 0;
    -webkit-box-sizing: border-box;
    box-sizing: border-box;
    text-decoration: none;
    list-style-type: none;
}
body {
    font-family: 'Roboto', 'Helvetica', 'Helvetica Neue', 'Arial', sans-serif;
}
.flex {
    display: flex;
}
.responsive-image {
    width: 100%;
    height: 100%;
}
.emoji {
    display: inline-block;
    width: 30px;
    height: 30px;
}
</style>
