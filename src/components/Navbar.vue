<template>
    <nav id="Navbar" class="navbar">
        <ul class="navLinks">
            <li><a href="#Home">Home</a></li>
            <li><a href="#About">About</a></li>
            <li><a href="#Projects">Projects</a></li>
            <li><a href="#Contact">Contacts</a></li>
        </ul>
    </nav>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .navbar {
        position: sticky;
        top: 0;
        z-index: 1;
        background: #1d1927;
        color: white;
        width: 100%;
        height: 3.5vh;
    }

    .navLinks {
        margin-top: 0;
        display: flex;  
        list-style: none;  
        margin-left: 18vh;    
    }

    li {
        margin-right: 8vh;
        font-size: 24px;
    }

    a {        
        text-decoration: none;
        color: white;
    }

    @media all and (max-width: 1024px) {
        .navbar {
            height: 115px;
        }
        
        .navLinks {
            flex-direction: column;
            justify-content: space-around;
            align-items: center;
            margin-left: 0;
        }
    }
    
</style>