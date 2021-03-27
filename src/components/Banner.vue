<template>
    <div id="Home" class="mainContainer">
        <p class="mainTitle">
            Hello World, I'm <span class="myName">Thomas Vandenbussche</span><br>
            I'm a fullstack JavaScript developer
        </p>
        <a class="toMyWorkButton" href="#Navbar">To my work →</a>
        <vue-particles
        class="particles"
        color="#dedede"
        :particleOpacity="0.7"
        :particlesNumber="100"
        shapeType="circle"
        :particleSize="4"
        linesColor="#dedede"
        :linesWidth="1"
        :lineLinked="true"
        :lineOpacity="0.4"
        :linesDistance="150"
        :moveSpeed="3"
        :hoverEffect="true"
        hoverMode="grab"
        :clickEffect="true"
        clickMode="push"
      />
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
        background: linear-gradient(to left, #040114, #0e548d);
        background-repeat: no-repeat;
        height: 100vh;
        color: white;
        font-weight: bold;
        align-items: center;
        justify-content: center;
    }

    .particles {
        position: absolute;
        top: 0;
        width: 100%;
        height: 100%;
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