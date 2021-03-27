<template>
    <div id="Contact" class="contactContainer">
        <div class="contactHeader">
            <p>Interested in working together? Just contact me with details about your project.</p>
            <div class="phoneAndMail">
                <p>
                    mail: <a href="mailto:thomas.vandenbussche@outlook.com">thomas.vandenbussche@outlook.com</a><br>
                    phone: <a href="tel:0603256652">+33(0)603256652</a>
                </p>
            </div>
        </div>
        <form>
            <input 
                id="from_name"
                placeholder="Your name"
                class="formInput" 
                type="text"><br>
            <input 
                id="from_mailAddress"
                placeholder="Your e-mail"
                class="formInput" 
                type="text"><br>
            <input 
                id="title"
                placeholder="Your subject"
                class="formInput" 
                type="text"><br>
            <textarea  
                itemid=""
                placeholder="Please share all you want here..."
                class="formInput" 
                name="" 
                id="message" 
                cols="30" 
                rows="10">
            </textarea>
            <button @click="sendMail" class="postMessageButton">Send</button>  
        </form>
            <div class="footerContact">
                <p>Thomas Vandenbussche®2021</p>
                <div>
                    <a href="mailto:thomas.vandenbussche@outlook.com">
                        <img class="contactIcons" src="../assets/mail.png" alt="LinkedIn icon">
                    </a>
                    <a href="https://www.linkedin.com/in/thomasvandenbussche/" target="_blank">
                        <img class="contactIcons" src="../assets/linkedin.png" alt="Linkedin logo">
                    </a>
                </div>
            </div>
    </div>
</template>

<script>
    import emailjs from 'emailjs-com';
    import{ init } from 'emailjs-com';
    import swal from 'sweetalert';

    init("user_SYFUzKPCMeVXcaAMzEzcM");
    
    export default {
        methods: {
            sendMail(e) {
                e.preventDefault()
                const tempParams = {
                    from_name: document.getElementById('from_name').value,
                    from_mailAddress: document.getElementById('from_mailAddress').value,
                    title: document.getElementById('title').value,
                    message: document.getElementById('message').value,
                }

                emailjs.send('service_kx5edij', 'template_h2pelur', tempParams)
                .then(function(res) {
                    console.log('success', res.status)
                })
                .then(
                    swal({
                        title: "Your mail just reached me !",
                        text: "Thank you for your message, I'll reply as soon as possible. Kindly, Thomas.",
                        icon: "success",
                    })
                )                
            }
        }
    }
</script>

<style scoped>
    .contactContainer {
        background: rgb(31, 15, 73);
        width: 100%;
        padding-top: 3vh;
    }

    .contactHeader {
        display: flex;
        justify-content: space-around;
        color: white;
    }

    .contactHeader > p {
        width: 45vh;
        font-size: 28px;
        margin-bottom: 5vh;
    }
    
    a {
        text-decoration: none;
        color: white;
    }

    a:hover {
        text-decoration: underline;
    }

    form {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .formInput {
        width: 80vh;
        border-radius: 5px;
    }

    .postMessageButton {
        justify-self: center;
        margin-top: 1.5vh;
        width: 8vh;
        height: 4vh;
        border-radius: 5px;
        background-color: rgb(28, 238, 109);
        font-size: 16px;
        font-weight: bold;
    }

    .footerContact {
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-top: 4vh;
        color: white;
    }

    .contactIcons {
        margin-right: 1vh;
        width: 6vh;
        height: 6vh;
    }
    
    @media all and (max-width: 1024px) {
        .formInput {
            width: 75%;
        }

        .contactHeader {
            flex-direction: column;
            text-align: center;
        }
    }
</style>
