<template>
    <div id="About" class="aboutContainer">
        <h2>About me</h2>
        <div class="myTalents">
            <div class="skill">
                <img class="icon" src="../assets/jsIcon.png" alt="Icon of JavaScript">
                <p>JavaScript (Vue / React)</p>
            </div>
            <div class="skill">
                <img class="icon" src="../assets/dbIcon.png" alt="Icon of a database">
                <p>Node.js with MongoDB, MySQL (Sequelize), Firebase</p>
            </div>
            <div class="skill">
                <img class="icon" src="../assets/mobileIcon.png" alt="Icon of a mobile phone">
                <p>Responsive</p>
            </div>
            <div class="skill">
                <img class="icon" src="../assets/agileIcon.png" alt="Icon of the agile methodology">
                <p>Agile methodology</p>
            </div>
            <div class="skill">
                <img class="icon" src="../assets/SEOIcon.png" alt="Icon of the SEO methodology">
                <p>Websites accessible and search engine optimized</p>
            </div>            
        </div>
        <div class="asideAbout">
            <div class="selfDescription">
                <img class="idPhoto" src="../assets/idPhoto.jpg" alt="Photo of Thomas">
                <p>I am a junior fullstack developer based in Paris (and ok to move) who just achieved the OpenClassrooms developer training. Working both front and back ends I can help you improve or build your website.</p>
            </div>
            <div class="knowledges">
                HTML 5
                <div class="meter">
                    <span style="width: 75%"></span>
                </div>
                CSS 3
                <div class="meter">
                    <span style="width: 70%"></span>
                </div>   
                JavaScript
                <div class="meter">                    
                    <span style="width: 65%"></span>
                </div> 
                Vue 3
                <div class="meter">                    
                    <span style="width: 65%"></span>
                </div>  
                React 7 / React Native
                <div class="meter">                    
                    <span style="width: 50%"></span>
                </div>  
                Node.js
                <div class="meter">                    
                    <span style="width: 65%"></span>
                </div>        
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .aboutContainer {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    h2 {
        font-size: 30px;
    }

    .myTalents {
        display: flex;
        justify-content: space-evenly;
    }

    .skill {
        width: 160px;
        margin: 4vh 2vh 0 2vh;
    }

    .skill > p {
        text-align: center;
        width: 75px;
    }

    .icon {
        width: 75px;
        height: 75px;
    }

    .selfDescription {
        width: 30vh;
        height: 50vh;
        margin-bottom: 12vh;
    }

    .selfDescription > p {
        width: 31vh;
        margin-bottom: 16vh;
    }

    .idPhoto {
        width: 300px;
        height: 300px;
    }

    .asideAbout {
        display: flex;
        margin-bottom: 11vh;
    }

    .knowledges {
        width: 35vh;
        margin: 3vh 0 0 35vh;
    }


    .meter {
        box-sizing: content-box;
        height: 20px; /* Can be anything */
        position: relative;
        margin-top: 3px;
        margin-bottom: 8px;
        background: rgb(97, 93, 93);
        border-radius: 25px;
        padding: 10px;
        box-shadow: inset 0 -1px 1px rgba(255, 255, 255, 0.3);
    }

    .meter > span {
        display: block;
        height: 100%;
        border-top-right-radius: 8px;
        border-bottom-right-radius: 8px;
        border-top-left-radius: 20px;
        border-bottom-left-radius: 20px;
        background-color: rgb(43, 194, 83);
        background-image: linear-gradient(
            center bottom,
            rgb(43, 194, 83) 37%,
            rgb(84, 240, 84) 69%
        );
        box-shadow: inset 0 2px 9px rgba(255, 255, 255, 0.3),
            inset 0 -2px 6px rgba(0, 0, 0, 0.4);
        position: relative;
        overflow: hidden;
    }

    @media all and (max-width: 1024px) {
        .myTalents {
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            margin: 0;
        }

        .skill {
            margin: 0;
            text-align: center;
        }

        .skill > p {
            width: 25vh;
        }

        .asideAbout {            
            flex-direction: column;
            justify-content: center;
        }

        .idPhoto {
            width: 33vh;
            height: 33vh;
        }

        .selfDescription {
            text-align: center;
        }

        .knowledges {
            margin: auto;
        }
    }

</style>