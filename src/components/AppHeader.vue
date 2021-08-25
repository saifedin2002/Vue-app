<template>
    <div class="header">
        <div class="container">
          <div id="logo">
            <router-link to="/">saifedin</router-link>
        </div>
        <ul class="text-right">
            <router-link to="/" exact>Home</router-link>
            <router-link to="/about">About</router-link>
            <router-link to="/blog" replace>Blog</router-link>
            <router-link to="/contact" replace>Contact</router-link>
        </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: "AppHeader",
};
</script>

<style lang="scss" scoped>
.header {
    background-color: #333;
    color: #fff;
    overflow: hidden;
    #logo {
        font-size: 24px;
        padding: 20px;
        width: 200px;
        float: left;
        display: block;
        a {
            color: #fff;
        }
    }
    ul {
        float: right;
        width: 500px;
        a {
            padding: 20px;
            color: #aeaeae;
            display: inline-block;
            font-size: 18px;
            &:hover,
            &:active {
                color: #fff;
                border-bottom: #fff solid 5px;
            }
        }
    }
}
</style>
