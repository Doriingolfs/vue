<template>
    <div id="top">
        <div id="logo">
        <img v-bind:src="'./assets/logo.png'">
        </div>
        <div id="button">
        <a href=""><div id="homes">
            <h1>{{ home }}</h1>
        </div></a>
        <a href=""><div id="companies">
            <h1>{{ company }}</h1>
        </div></a>
        <a href=""><div id="housings">
            <h1>{{ housing }}</h1>
        </div></a>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'header',

        data: () => ({
            home: 'Heimili',
            company: 'Fyrirtæki',
            housing: 'Húsfélög',      
        })
    }
</script>

<style lang="scss" scoped>
    #logo {
        width: 50%;
        float: left;
    }
    #top {
        height: 500px;
        padding-top: 100px;
    }
    img {
        height: 100px;
        width: 100px;
    }
    #button {
        float: right;
        width: 50%;
    }
    #homes {
        background-color: #066766;
        font-size: 24px;
        height: 90px;
        padding: 10px 10px 10px 30px;
    }
    #companies {
        background-color: #099795;
        font-size: 24px;
        height: 90px;
        padding: 10px 10px 10px 30px;
    }
    #housings {
        background-color: #066766;
        font-size: 24px;
        height: 90px;
        padding: 10px 10px 10px 30px;
    }
    #button :hover{
        margin-left: -40px;
        transition: 0.6s;
        cursor: pointer;
    }
</style>