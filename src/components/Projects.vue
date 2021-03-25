<template>
    <div class="projectsContainer">
        <h2>My Projects</h2>
        <div class="projects">
            <div
                id="CV"
                class="project cv"
                @mouseover="hoverCV" 
                @mouseleave="leaveCV" 
            >  
                <h1 id="cvTitle"></h1>
                <p id="cvDescription"></p>
                <p id="cvLink"></p>
            </div>
            <div 
                id="ohMyFood"
                class="project ohMyFood"
                @mouseover="hoverOhMyFood" 
                @mouseleave="leaveOhMyFood" 
            >
                <h1 id="ohMyFoodTitle"></h1>
                <p id="ohMyFoodDescription"></p>
                <p id="ohMyFoodLink"></p>
            </div>
            <div 
                id="laChouetteAgence"
                class="project laChouetteAgence"
                @mouseover="hoverLaChouetteAgence" 
                @mouseleave="leaveLaChouetteAgence" 
            >
                <h1 id="laChouetteAgenceTitle"></h1>
                <p id="laChouetteAgenceDescription"></p>
                <p id="laChouetteAgenceLink"></p>
            </div>
            <div
                id="orinobear"
                class="project orinobear"
                @mouseover="hoverOrinobear" 
                @mouseleave="leaveOrinobear"
            >
                <h1 id="orinobearTitle"></h1>
                <p id="orinobearDescription"></p>
                <p id="orinobearLink"></p>
            </div>
            <div
                id="essentiallyOils"
                class="project essentiallyOils"
                @mouseover="hoverEssentiallyOils" 
                @mouseleave="leaveEssentiallyOils"
            >
                <h1 id="essentiallyOilsTitle"></h1>
                <p id="essentiallyOilsDescription"></p>
                <p id="essentiallyOilsLink"></p>
            </div>
            <div
                id="oikoPolis"
                class="project oikoPolis"
                @mouseover="hoverOikoPolis" 
                @mouseleave="leaveOikoPolis" 
            >
                <h1 id="oikoPolisTitle"></h1>
                <p id="oikoPolisDescription"></p>
                <p id="oikoPolisLink"></p>
            </div>
            <div 
                id="soPecocko"
                class="project soPecocko"
                @mouseover="hoverSoPecocko" 
                @mouseleave="leaveSoPecocko" 
            >
                <h1 id="soPecockoTitle"></h1>
                <p id="soPecockoDescription"></p>
                <p id="soPecockoLink"></p>
            </div>
            <div 
                id="moviesAndMe"
                class="project moviesAndMe"
                @mouseover="hoverMoviesAndMe" 
                @mouseleave="leaveMoviesAndMe"               
            >
                <h1 id="moviesAndMeTitle"></h1>
                <p id="moviesAndMeDescription"></p>
                <p id="moviesAndMeLink"></p>
            </div>
            <div
                id="rpProject"
                class="project rpProject"
                @mouseover="hoverRpProject" 
                @mouseleave="leaveRpProject"
            >
                <h1 id="rpProjectTitle"></h1>
                <p id="rpProjectDescription"></p>
                <p id="rpProjectLink"></p>
            </div>
        </div>        
    </div>
</template>

<script>
    export default {
        methods: {            
            hoverCV() {
                const cv = document.getElementById('CV')
                const cvTitle = document.getElementById('cvTitle')
                const cvDescription = document.getElementById('cvDescription')
                const cvLink = document.getElementById('cvLink')
                cv.className="hoveredProject"
                cvTitle.innerHTML = 'Curriculum Vitae'
                cvDescription.innerHTML = 'Very first OpenClassrooms Project to learn HTML and CSS with Flexbox and the rules of responsive design.'
                cvLink.innerHTML = "Access the website →"
                cvLink.style.border="solid white 2px"
                cvLink.style.padding="6px"
                cvLink.style.cursor = "pointer"
                cvLink.addEventListener('click', function() {
                    window.open(
                        "https://vandethom.github.io/OikoPolis/index.html",
                        '_blank'
                    ) 
                })
            },
            leaveCV() {
                const cv = document.getElementById('CV')
                const cvTitle = document.getElementById('cvTitle')
                const cvDescription = document.getElementById('cvDescription')
                const cvLink = document.getElementById('cvLink')
                cv.className="project cv"
                cvTitle.innerHTML = ""
                cvDescription.innerHTML = ""
                cvLink.innerHTML = ""
                cvLink.style="none"
            },
            hoverOhMyFood() {
                const ohMyFood = document.getElementById('ohMyFood')
                const ohMyFoodTitle = document.getElementById('ohMyFoodTitle')
                const ohMyFoodDescription = document.getElementById('ohMyFoodDescription')
                const ohMyFoodLink = document.getElementById('ohMyFoodLink')
                ohMyFood.className="hoveredProject"
                ohMyFoodTitle.innerHTML = 'Oh My Food'
                ohMyFoodDescription.innerHTML = 'Second project in order to practice more CSS, with SCSS pre-processor and deepen knowledge of VSC extensions.'
                ohMyFoodLink.innerHTML = "Access the website →"
                ohMyFoodLink.style.border="solid white 2px"
                ohMyFoodLink.style.padding="6px"
                ohMyFoodLink.style.cursor = "pointer"
                ohMyFoodLink.addEventListener('click', function() {
                    window.open(
                        "https://vandethom.github.io/ohmyfood/index.html",
                        '_blank'
                    ) 
                })
            },
            leaveOhMyFood() {
                const ohMyFood = document.getElementById('ohMyFood')
                const ohMyFoodTitle = document.getElementById('ohMyFoodTitle')
                const ohMyFoodDescription = document.getElementById('ohMyFoodDescription')
                const ohMyFoodLink = document.getElementById('ohMyFoodLink')
                ohMyFood.className="project ohMyFood"
                ohMyFoodTitle.innerHTML = ""
                ohMyFoodDescription.innerHTML = ""
                ohMyFoodLink.innerHTML = ""
                ohMyFoodLink.style="none"
            },
            hoverLaChouetteAgence() {
                const laChouetteAgence = document.getElementById('laChouetteAgence')
                const laChouetteAgenceTitle = document.getElementById('laChouetteAgenceTitle')
                const laChouetteAgenceDescription = document.getElementById('laChouetteAgenceDescription')
                const laChouetteAgenceLink = document.getElementById('laChouetteAgenceLink')
                laChouetteAgence.className="hoveredProject"
                laChouetteAgenceTitle.innerHTML = 'La Chouette Agence'
                laChouetteAgenceDescription.innerHTML = 'Focusing on SEO and web accessibility, this project taught how to make a website faster, accessible to anybody and, the most important : make it visible on search engines and social medias !'
                laChouetteAgenceLink.innerHTML = "Access the website →"
                laChouetteAgenceLink.style.border="solid white 2px"
                laChouetteAgenceLink.style.padding="6px"
                laChouetteAgenceLink.style.cursor = "pointer"
                laChouetteAgenceLink.addEventListener('click', function() {
                    window.open(
                        "https://vandethom.github.io/LaChouetteAgenceSEO/",
                        '_blank'
                    ) 
                })
            },
            leaveLaChouetteAgence() {
                const laChouetteAgence = document.getElementById('laChouetteAgence')
                const laChouetteAgenceTitle = document.getElementById('laChouetteAgenceTitle')
                const laChouetteAgenceDescription = document.getElementById('laChouetteAgenceDescription')
                const laChouetteAgenceLink = document.getElementById('laChouetteAgenceLink')
                laChouetteAgence.className="project laChouetteAgence"
                laChouetteAgenceTitle.innerHTML = ""
                laChouetteAgenceDescription.innerHTML = ""
                laChouetteAgenceLink.innerHTML = ""
                laChouetteAgenceLink.style = "none"
            },
            hoverOrinobear() {
                const orinobear = document.getElementById('orinobear')
                const orinobearTitle = document.getElementById('orinobearTitle')
                const orinobearDescription = document.getElementById('orinobearDescription')
                const orinobearLink = document.getElementById('orinobearLink')
                orinobear.className="hoveredProject"
                orinobearTitle.innerHTML = 'Orinobear'
                orinobearDescription.innerHTML = 'OpenClassrooms project 4, first step in native JavaScript with Bootstrap to build an e-commerce website selling teddies fetched from a database. Unfortunately, the back-end is not yet available (I\'ll dispatch it on Firebase soon), so the website it not entirely visible.'
                orinobearLink.innerHTML = "Access the website →"
                orinobearLink.style.border="solid white 2px"
                orinobearLink.style.padding="6px"
                orinobearLink.style.cursor = "pointer"
                orinobearLink.addEventListener('click', function() {
                    window.open(
                        "https://vandethom.github.io/Oribear/",
                        '_blank'
                    ) 
                })
            },
            leaveOrinobear() {
                const orinobear = document.getElementById('orinobear')
                const orinobearTitle = document.getElementById('orinobearTitle')
                const orinobearDescription = document.getElementById('orinobearDescription')
                const orinobearLink = document.getElementById('orinobearLink')
                orinobear.className="project orinobear"
                orinobearTitle.innerHTML = ""
                orinobearDescription.innerHTML = ""
                orinobearLink.innerHTML = ""
                orinobearLink.style = "none"
            },
            hoverEssentiallyOils() {
                const essentiallyOils = document.getElementById('essentiallyOils')
                const essentiallyOilsTitle = document.getElementById('essentiallyOilsTitle')
                const essentiallyOilsDescription = document.getElementById('essentiallyOilsDescription')
                const essentiallyOilsLink = document.getElementById('essentiallyOilsLink')
                essentiallyOils.className="hoveredProject"
                essentiallyOilsTitle.innerHTML = 'Essentially Oils'
                essentiallyOilsDescription.innerHTML = 'My very first own project ! Cloning Amazon to make it more nature friendly. Using React with Redux for the front and Firebase for the back, you can create an account, add an item to your cart, delete it or even pay it with your credit card.'
                essentiallyOilsLink.innerHTML = "Access the website →"
                essentiallyOilsLink.style.border="solid white 2px"
                essentiallyOilsLink.style.padding="6px"
                essentiallyOilsLink.style.cursor = "pointer"
                essentiallyOilsLink.addEventListener('click', function() {
                    window.open(
                        "https://essential-7fc0d.web.app/",
                        '_blank'
                    ) 
                })
            },
            leaveEssentiallyOils() {
                const essentiallyOils = document.getElementById('essentiallyOils')
                const essentiallyOilsTitle = document.getElementById('essentiallyOilsTitle')
                const essentiallyOilsDescription = document.getElementById('essentiallyOilsDescription')
                const essentiallyOilsLink = document.getElementById('essentiallyOilsLink')
                essentiallyOils.className="project essentiallyOils"
                essentiallyOilsTitle.innerHTML = ""
                essentiallyOilsDescription.innerHTML = ""
                essentiallyOilsLink.innerHTML = ""
                essentiallyOilsLink.style = "none"
            },
            
            hoverOikoPolis() {
                const oikoPolis = document.getElementById('oikoPolis')
                const oikoPolisTitle = document.getElementById('oikoPolisTitle')
                const oikoPolisDescription = document.getElementById('oikoPolisDescription')
                const oikoPolisLink = document.getElementById('oikoPolisLink')
                oikoPolis.className="hoveredProject"
                oikoPolisTitle.innerHTML = 'Clé de Voûte'
                oikoPolisDescription.innerHTML = 'A showcase website in HTML and CSS / SCSS ordered to me by real estate students in Paris. A good occasion to train a bit more with the pre-processor !'
                oikoPolisLink.innerHTML = "Access the website →"
                oikoPolisLink.style.border="solid white 2px"
                oikoPolisLink.style.padding="6px"
                oikoPolisLink.style.cursor = "pointer"
                oikoPolisLink.addEventListener('click', function() {
                    window.open(
                        "https://vandethom.github.io/OikoPolis/index.html",
                        '_blank'
                    ) 
                })                
            },
            leaveOikoPolis() {
                const oikoPolis = document.getElementById('oikoPolis')
                const oikoPolisTitle = document.getElementById('oikoPolisTitle')
                const oikoPolisDescription = document.getElementById('oikoPolisDescription')
                const oikoPolisLink = document.getElementById('oikoPolisLink')
                oikoPolis.className="project oikoPolis"
                oikoPolisTitle.innerHTML = ""
                oikoPolisDescription.innerHTML = ""
                oikoPolisLink.innerHTML = ""
                oikoPolisLink.style = "none"
            },
            hoverSoPecocko() {
                const soPecocko = document.getElementById('soPecocko')
                const soPecockoTitle = document.getElementById('soPecockoTitle')
                const soPecockoDescription = document.getElementById('soPecockoDescription')
                const soPecockoLink = document.getElementById('soPecockoLink')
                soPecocko.className="hoveredProject"
                soPecockoTitle.innerHTML = 'So Pecocko'
                soPecockoDescription.innerHTML = 'Fifth project of OpenClassrooms creating an API with Express and MongoDB to find a sauce and like or dislike it.'
                soPecockoLink.innerHTML = "Access the website →"
                soPecockoLink.style.border="solid white 2px"
                soPecockoLink.style.padding="6px"
                soPecockoLink.style.cursor = "pointer"
                soPecockoLink.addEventListener('click', function() {
                    window.open(
                        "https://github.com/Vandethom/SoPecocko",
                        '_blank'
                    ) 
                })               
            },
            leaveSoPecocko() {
                const soPecocko = document.getElementById('soPecocko')
                const soPecockoTitle = document.getElementById('soPecockoTitle')
                const soPecockoDescription = document.getElementById('soPecockoDescription')
                const soPecockoLink = document.getElementById('soPecockoLink')
                soPecocko.className="project ohMyFood"
                soPecockoTitle.innerHTML = ""
                soPecockoDescription.innerHTML = ""
                soPecockoLink.innerHTML = ""
                soPecockoLink.style = "none"
            },
            hoverMoviesAndMe() {
                const moviesAndMe = document.getElementById('moviesAndMe')
                const moviesAndMeTitle = document.getElementById('moviesAndMeTitle')
                const moviesAndMeDescription = document.getElementById('moviesAndMeDescription')
                const moviesAndMeLink = document.getElementById('moviesAndMeLink')
                moviesAndMe.className="hoveredProject"
                moviesAndMeTitle.innerHTML = 'Movies And Me'
                moviesAndMeDescription.innerHTML = 'First try on React Native to create a MovieSearch app searching and keep favorites in db. Created with TheMovieDataBase API.'
                moviesAndMeLink.innerHTML = "Access the website →"
                moviesAndMeLink.style.border="solid white 2px"
                moviesAndMeLink.style.padding="6px"
                moviesAndMeLink.style.cursor = "pointer"
                moviesAndMeLink.addEventListener('click', function() {
                    window.open(
                        "https://github.com/Vandethom/MoviesAndMe",
                        '_blank'
                    ) 
                })               
            },
            leaveMoviesAndMe() {
                const moviesAndMe = document.getElementById('moviesAndMe')
                const moviesAndMeTitle = document.getElementById('moviesAndMeTitle')
                const moviesAndMeDescription = document.getElementById('moviesAndMeDescription')
                const moviesAndMeLink = document.getElementById('moviesAndMeLink')
                moviesAndMe.className="project moviesAndMe"
                moviesAndMeTitle.innerHTML = ""
                moviesAndMeDescription.innerHTML = ""
                moviesAndMeLink.innerHTML = ""
                moviesAndMeLink.style = "none"
            },
            hoverRpProject() {
                const rpProject = document.getElementById('rpProject')
                const rpProjectTitle = document.getElementById('rpProjectTitle')
                const rpProjectDescription = document.getElementById('rpProjectDescription')
                const rpProjectLink = document.getElementById('rpProjectLink')
                rpProject.className="hoveredProject"
                rpProjectTitle.innerHTML = 'A Personal roleplay API'
                rpProjectDescription.innerHTML = 'A try with Sequelize in a Node express API to create an API able to render characters sheet in a role play.'
                rpProjectLink.innerHTML = "Access the website →"
                rpProjectLink.style.border="solid white 2px"
                rpProjectLink.style.padding="6px"
                rpProjectLink.style.cursor = "pointer"
                rpProjectLink.addEventListener('click', function() {
                    window.open(
                        "https://github.com/Vandethom/RP-API",
                        '_blank'
                    ) 
                })               
            },
            leaveRpProject() {
                const rpProject = document.getElementById('rpProject')
                const rpProjectTitle = document.getElementById('rpProjectTitle')
                const rpProjectDescription = document.getElementById('rpProjectDescription')
                const rpProjectLink = document.getElementById('rpProjectLink')
                rpProject.className="project rpProject"
                rpProjectTitle.innerHTML = ""
                rpProjectDescription.innerHTML = ""
                rpProjectLink.innerHTML = ""
                rpProjectLink.style = "none"
            },
        }
    }
</script>

<style scoped>
    .projectsContainer {
        background: rgb(236, 232, 232);
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .projects {
        width: 66%;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
    }

    img {
        width: 350px;
        height: 350px;
        transition: transform 0.7s;
    }

    img:hover {
        transform: scale(1.2);
    }

    .project {
        margin-bottom: 3vh;
        border-radius: 15%;
        width: 350px;
        height: 350px;
        transition: transform 0.7s;
        transform: scale(1);
    }

    .hoveredProject {
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
        padding: 5px;
        border-radius: 15%;
        background: rgb(21, 19, 155);
        color: white;
        width: 350px;
        height: 350px;
        transform: scale(1.1);
        transition: transform 0.7s;
    }

    .skillButton {
        border: 2px solid white;
    }
    
    .cv {
        background-image: url('../assets/cv.png');
        background-size: 350px;
    }

    .ohMyFood {
        background-image: url('../assets/ohMyFood.png');
        background-size: 350px;
    }

    .laChouetteAgence {
        background-image: url('../assets/laChouetteAgence.png');
        background-size: 350px;
    }

    .orinobear {
        background-image: url('../assets/orinobear.png');
        background-size: 350px;
    }

    .essentiallyOils {
        background-image: url('../assets/essentiallyOils.png');
        background-size: 350px;
    }

    .oikoPolis {
        background-image: url('../assets/oikoPolis.png');
        background-size: 350px;
    }
    
    .soPecocko {
        background-image: url('../assets/soPecocko.png');
        background-size: 350px;
    }

    .moviesAndMe {
        background-image: url('../assets/moviesAndMe.png');
        background-size: 350px;
    }

    .rpProject {
        background-image: url('../assets/rp-project.png');
        background-size: 350px;
    }
</style>
    