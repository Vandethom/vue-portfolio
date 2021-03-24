<template>
    <div id="Home" class="mainContainer">
        <p class="mainTitle">
            Hello World, I'm <span class="myName">Thomas Vandenbussche</span><br>
            I'm a fullstack JavaScript developer
        </p>
        <a class="toMyWorkButton" href="#Navbar">To my work →</a>
    </div>
</template>

<script>

    export default {

    }
</script>

<style scoped>
    .mainContainer {
        margin-bottom: 0;
        display: flex;
        flex-direction: column;
        background-image: url('../assets/background.png');
        background-repeat: no-repeat;
        height: 100vh;
        color: white;
        font-weight: bold;
        align-items: center;
        justify-content: center;
    }

    .mainTitle {
        font-size: 36px;
    }

    .myName {
        font-size: 40px;
        color: #12aa26;
    }

    .toMyWorkButton {
        text-decoration: none;
        color: white;
        border: 2px solid white;
        padding: 1.5vh;
        font-size: 26px;
    }
</style>