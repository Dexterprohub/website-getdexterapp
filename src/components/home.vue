<template>
    <div class="container">
        <div class="header">
            <nav>
                <ul class="logoul">
                    <li><router-link to="/"><img src="../assest/images/home/Logo.png" alt="Company Logo" class="logo"></router-link></li>
                    <li>
                        <img src="../assest/images/icon-menu-close.svg" alt="" class="close" ref="close" @click="close">
                        <img src="../assest/images/icon-menu.svg" alt="" class="menu" ref="menu" @click="open">
                    </li>
                    <li>
                        <ul class="navbar" ref="navbar">
                            <li><router-link to="/">Home</router-link></li>
                            <li><router-link to="#">About</router-link></li>
                            <li><router-link to="/business">For Business</router-link></li>
                            <li><router-link to="#">FAQs</router-link></li>
                        </ul>
                    </li>
                </ul>
            </nav>
            <div class="hero-section">
                <div class="hero">
                    <h1>Save time Outsourcing <br /> Daily Tasks</h1>
                    <p>Do you have any task or chore you want done anywhere, The Dexter App provides you with a pool<br />
                        of
                        services to pick from. Get qualified service personnel assigned to your tasks in minutes.</p>
                    <button>Join Waitlist</button>
                    <div class="hero-images" ref="imageRotate">
                        <img src="../assest/images/home/hero-img1.png" alt="" class="hero-img1">
                        <img src="../assest/images/home/hero-img2.png" alt="" class="hero-img2">
                    </div>

                </div>
            </div>
        </div>

        <main>
            <div class="services-container">
                <div class="service-discription">
                    <h1>Discover Our Services</h1>
                    <p>We cover a whole lot of services and we are still adding more to the list</p>
                </div>
                <div class="services">
                    <div class="services_info">
                        <img src="../assest/images/home/electricity.png" alt=""><br />
                        <h3>Electrical Repair</h3>
                    </div>
                    <div class="services_info">
                        <img src="../assest/images/home/laundry.png" alt="">
                        <h3>Laundry</h3>
                    </div>
                    <div class="services_info">
                        <img src="../assest/images/home/food.png" alt="">
                        <h3>Food Delivery</h3>
                    </div>
                    <div class="services_info">
                        <img src="../assest/images/home/makeup.png" alt=""><br />
                        <h3>Make up</h3>
                    </div>
                    <div class="services_info">
                        <img src="../assest/images/home/plumbing.png" alt="">
                        <h3>Plumbing</h3>
                    </div>
                    <div class="services_info">
                        <img src="../assest/images/home/grocery.png" alt="">
                        <h3>Grocery Shopping</h3>
                    </div>
                    <div class="services_info">
                        <img src="../assest/images/home/hair-styling.png" alt="">
                        <h3>Hair Styling</h3>
                    </div>
                    <div class="services_info">
                        <img src="../assest/images/home/fashion-design.png" alt="">
                        <h3>Fashion Design</h3>
                    </div>
                </div>

            </div>
            <div class="location">
                
                <h1>
                    <span class="mainh1">Currently available in: </span>
                    <br />
                    <span class="sech1">
                        <img src="../assest/images/home/flag.png" alt="">
                            <span class="location-discription">Lagos, Nigeria</span>
                    </span>
                </h1>
                
                <p>Our goal is to bring Dexter to as many states as possible in Nigeria.<br /> We’re just getting
                    started. <span><a href="#" class="news">Join our newsletter</a></span> to recieve updates from
                    Dexter<br /> as soon as our
                    services are
                    available in your state or area.</p>
            </div>
            <div class="signUp">
                <img src="../assest/images/home/signupImg.png" alt="" class="iphone">
                <div class="min-signup">
                    <h1>Sign up for our Beta Launch</h1>
                    <ul>
                        <li><img src="../assest/images/home/download.png" alt="">
                            <h6> Click on the “Join Waitlist” button on the website</h6>
                        </li>
                        <li><img src="../assest/images/home/info.png" alt="">
                            <h6>Fill in your information</h6>
                        </li>
                        <li><img src="../assest/images/home/star.png" alt="">
                            <h6>A confirmation email will be sent to you</h6>
                        </li>
                    </ul>
                    <button>Join Waitlist</button>
                </div>
            </div>
            <div class="support">
                <div>
                    <h1>Our support team is always ready to help</h1>
                    <p>Trust and credibility is a single item on our list, our support team are a mix of supply chain
                        experts and IT professionals always ready to guide you through any concerns you may have. You won’t
                        be having issues with Dexter but we are doing this incase...</p>
                    <button><a href="#"></a>Contact Us</button>
                </div>
                <img src="../assest/images/home/peopletree.png" alt="">
            </div>
            <div class="newsletter">
                <div class="newsletter-details">
                    <h1>Stay updated with our Newsletter</h1>
                    <p>Be the first to receive our latest news, updates and everything in between.</p>
                </div>
                <div class="newsletter-signup">
                    <input type="Email" placeholder="Your Mail">
                    <button><a href="#">Signup</a></button>
                </div>
            </div>
        </main>

    </div>
    <footer>
        <div class="socials">
            <img src="../assest/images/home/Logo.png" alt="Company Logo" class="logo2">
            <p>© 2023 Dexterprolimited. All rights reserved</p>
            <ul>
                <li><a href="#"><img src="../assest/images/home/instagram.png" alt=""></a></li>
                <li><a href="#"><img src="../assest/images/home/twitter.png" alt=""></a></li>
                <li><a href="#"><img src="../assest/images/home/Youtube.png" alt=""></a></li>
                <li><a href="#"><img src="../assest/images/home/linkedin.png" alt=""></a></li>
            </ul>
        </div>
        <div class="links">
            <h1>Quick Links</h1>
            <ul>
                <li><router-link to="/about">About</router-link></li>
                <li><router-link to="/contact">Contact</router-link> </li>
                <li><router-link to="/faq">FAQs</router-link> </li>
                <li><router-link to="/termOfServices">Term Of Service</router-link> </li>
                <li><router-link to="/ImageCredits">Image Credits</router-link></li>
            </ul>
        </div>
        <div class="contactus">
            <h1>Contact</h1>
            <ul>
                <li><img src="../assest/images/home/mail.png" alt="">
                    <p>support@dexterapp.com</p>
                </li>
                <li><img src="../assest/images/home/tel.png" alt="">
                    <p>+ 1 628 900 2879</p>
                </li>
                <li><img src="../assest/images/home/location.png" alt="">
                    <p>36b, Jay Jay Oladimeji Street, off. Freedom Way, Ikate Lekki, Lagos State</p>
                </li>
            </ul>

        </div>
    </footer>
</template>

<script>

export default {
    name: 'home',
    data() {
        return {

        }
    },
    methods: {
        open() {
            if (this.$refs.navbar.style.display = 'none') {
                this.$refs.navbar.style.display = 'block'
                this.$refs.close.style.display = 'block'
                this.$refs.menu.style.display = 'none'


            }
        },
        close() {
            if (this.$refs.navbar.style.display = 'block') {
                this.$refs.navbar.style.display = 'none'
                this.$refs.menu.style.display = 'block'
                this.$refs.close.style.display = ' none'
            }
        }

    }
}

</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Manrope:wght@600&display=swap');


* {
    font-family: 'Manrope';
    color: #000000;
}

h1 {
    color: #000000;
}

.header {
    background-image: url('../assest/images/home/background.png');
    background-color: #276E59;
    background-repeat: no-repeat;
    background-size: cover;
    padding: 5vh 10vw 5vh 10vw;
}

.close,
.menu {
    display: none;
}

nav img {
    cursor: pointer;
}

nav ul {
    display: flex;
    justify-content: space-between;
    list-style: none;

}

.navbar {
    display: flex;
    justify-content: space-between;
    gap: 2vw;
    font-family: 'Manrope', sans-serif;
    font-size: 16px;
}

a {
    text-decoration: none;
    color: #FFFFFF;
}

.navbar a.router-link-active {
    color: #FFFFFF;
    text-decoration: none;
}

.hero-section {
    text-align: center;
    font-family: 'manrope', sans-serif;
    position: relative;
}

.hero h1 {
    font-weight: 800;
    color: #FFFFFF;
}

.hero p {
    color: #FFFFFF;
    font-weight: 400;
    font-size: 18px;
    line-height: 24.59px;
}

.hero button {
    background-color: #000000;
    color: #FFFFFF;
    border-radius: 30px;
    border: none;
    padding-top: 2vh;
    padding-bottom: 2vh;
    cursor: pointer;
}

.hero-images {
    margin-top: 10vh;
    margin-left: 3vw;
}

.services-container {
    background-color: #FAFAFA;
    text-align: center;
    padding-bottom: 10vh;
}


.service-discription p {
    margin-top: 0;
    font-weight: 400;
    font-size: 18px;
    color: #5B5B5B;
}


.service-discription h1 {
    margin: 0;
}

.services {
    margin: 5vh 5vh 2vh 4vw;
}

.services_info {
    height: 242px;
    background-color: #FFFFFF;
    text-align: left;
}

.services_info img,
h3 {
    margin: 8vh 2vw 0 2vw;
}


.location {
    background-color: #E6E6E6;
    text-align: center;
    margin: 0;
    padding: 10vh 10vw 10vh 10vw;
}

.location h1 {
    font-size: 40px;
    margin: 0;
}

.location-discription {
    color: #131313;
    font-weight: 700;
    font-size: 20px;
}

.news {
    color: #276E59;
}

.location p {
    margin-top: 5vh;
    color: #5B5B5B;
    font-size: 18px;
    font-weight: 400;
    line-height: 24.59px;
}

.mainh1 {
    color: #131313;
}

.sech1 {
    position: relative;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 8px;
}


.signupImg {
    position: absolute;
    left: 325px;
    top: 120;
    border-radius: 5%;
}

.min-signup {
    margin-top: 10vh;
}

.min-signup h1 {
    color: #131313;

}

.min-signup ul {
    list-style: none;
    margin: 0;
    padding: 0;
}

.min-signup ul li img {
    margin-right: 2vw;
    margin: 0 2vw 0 0vw;
}

.min-signup ul li h6 {
    font-size: 20px;
    color: #131313;
    margin: 1vh 0 0 0;
}

.min-signup button {
    width: 20vw;
    border: none;
    background-color: #000000;
    color: #FFFFFF;
    border-radius: 30px;
    padding-top: 2vh;
    padding-bottom: 2vh;
    cursor: pointer;
    margin-left: 5vw;
}

.support {
    background-image: url('../assest/images/home/background.png');
    background-color: #276E59;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    gap: 10vw;
    padding: 10vh 12vw 10vh 12vw;
    text-align: center;
}

.support div {
    margin-top: 10vh;
}

.support div h1 {
    color: #FFFFFF;
    font-size: 40px;
    font-weight: 700;
    line-height: 50px;
}

.support div p {
    color: #FAFAFA;
    font-weight: 400;
    font-size: 18px;
    line-height: 24.59px;
}

.support button {
    background-color: #EBA53B;
    width: 20vw;
    border: none;
    border-radius: 30px;
    padding-top: 2vh;
    padding-bottom: 2vh;
    cursor: pointer;
}

.support button a {
    text-decoration: none;
    color: #131313;
}

.support img {
    border-right: 10px solid #EDC700;
    border-bottom: 10px solid #EDC700;
    border-bottom-right-radius: 30px;
    border-top-right-radius: 30px;
    border-bottom-left-radius: 30px;
}

.newsletter {
    position: relative;
    background-color: #276E59;
    display: grid;
    grid-template-columns: 40vw 20vw;
    margin: 10vh 10vw 0vh 10vw;
    padding: 5vh 7vw 5vh 5vw;
    gap: 3vw;
    border-radius: 15px;
    top: 20vh;
}

.newsletter-details {
    color: #FFFFFF;
}

.newsletter-details h1 {
    font-size: 40px;
    font-weight: 700px;
    line-height: 50px;
    color: #FFFFFF;
}

.newsletter-details p {
    color: #FAFAFA;
    font-weight: 400;
    font-size: 18px;
}

.newsletter-signup {
    display: grid;
    grid-template-rows: 20vw, 20vw;
    gap: 2vh;
    margin: 5vh 0 5vh 0;
}

.newsletter-signup input {
    height: 50px;
    border: 1px solid #D6D8DB;
    border-radius: 30px;
    padding-left: 2vw;

}

.newsletter-signup button {
    width: 20vw;
    border: none;
    background-color: #EBA53B;
    color: #FFFFFF;
    border-radius: 30px;
    cursor: pointer;
    padding-top: 2vh;
    padding-bottom: 2vh;
}

footer {
    background-color: #0B0D17;
    color: #FEFEFE;
    display: grid;
    margin: 0;
    grid-template-columns: 40vw 22vw 22vw;
    padding: 15vw 5vw 5vw 5vw;

}

footer h1 {
    color: #FEFEFE;
    margin: 0;
}

footer ul {
    list-style: none;
    padding: 0;
}

.socials p {
    color: #D9DBE1;
    font-weight: 400;
    font-size: 14px;
}

.socials {
    text-align: left;
}

.socials ul {
    list-style: none;
    display: flex;
    gap: 1vw;
}

.links h1 {
    font-weight: 700;
    font-size: 20px;
    color: #FEFEFE;
}

.links ul li {
    margin-bottom: 1.5vh;
}

.links ul li a {
    color: #D9DBE1;
    font-size: 14px;
    font-weight: 400;

}

.contactus h1 {
    color: #FFFFFF;
    font-size: 20px;
    font-weight: 700;
}

.contactus ul li {
    display: grid;
    grid-template-columns: 2vw 15vw;
    gap: .5vw;
    margin-bottom: 2vh;
}

.contactus ul li p {
    margin: 0;
    font-size: 14px;
    font-weight: 400;
    color: #D9DBE1;
}



@media screen and (min-width: 913px) {
    a {
        font-size: 18px;
    }

    .hero h1 {
        font-size: 64px;
        line-height: 70.14px;
    }

    .hero button {
        margin-top: 5vh;
        width: 342px;
        padding-top: 2.5vh;
        padding-bottom: 2.5vh;
    }

    .hero-images {
        display: flex;
    }

    .hero-img1 {
        position: relative;
        left: 18vw;
    }

    .hero-img2 {
        position: relative;
        left: 4vw;
    }


    .services {
        display: grid;
        grid-template-columns: repeat(4, 274.5px);
        gap: 2vw;
        margin: 5vh 10vw 2vh 10vw;

    }

    .services_info img {
        margin: 5vh 2vw 0 2vw;
    }

    .services_info h3 {
        margin: 2vh 2vw 0 2vw;
        color: #1B1D21;
    }

    .service-discription {
        padding-top: 5vh;
    }

    .service-discription h1 {
        font-weight: 700;
        font-size: 40px;
    }

    .signUp {
        padding: 10vh 10vw 10vh 10vw;
        display: grid;
        grid-template-columns: 31vw 40vw;
        gap: 5vw;
    }

    .min-signup {
        margin-top: 3vh;
    }

    .min-signup ul li {
        margin: 0;
        margin-bottom: 3vh;
        padding: 0;
        display: grid;
        grid-template-columns: 2vw 25vw;
        gap: 5vw;
    }

    .min-signup h1 {
        color: #131313;
        font-size: 40px;
        font-weight: 700;
    }

    .min-signup button {
        width: 30vw;
        margin-top: 5vh;
        margin-left: 0;
        padding-top: 2.5vh;
        padding-bottom: 2.5vh;
    }

    .mainh1 {
        font-size: 40px;
    }

    .support {
        background-image: url('../assest/images/home/background.png');
        background-color: #276E59;
        background-repeat: no-repeat;
        background-size: cover;
        display: grid;
        grid-template-rows: none;
        grid-template-columns: 30vw 30vw;
        gap: 20vh;
        padding: 10vh 10vw 10vh 10vw;
    }

    .support div {
        margin-top: 5vh;
    }

    .support div button {
        width: 20vw;
        padding-top: 2vh;
        padding-bottom: 2vh;
        font-size: 18px;
    }

    .newsletter {
        top: 15vh;
    }

    .newsletter-signup {
        margin: 3vh 0 5vh 0;
    }

    .newsletter-signup button {
        padding-top: 1.5vh;
        padding-bottom: 1.5vh;
        width: 25vw;
    }

    .newsletter-signup input {
        padding: 0 0 0 2vw;
    }

    .newsletter-details h1 {
        font-size: 30px;
        line-height: 40px;
    }

    footer {
        padding-top: 20vh;
        grid-template-columns: 40vw 22vw 25vw;
    }

    .contactus ul li {
        grid-template-columns: 2vw 20vw;
        gap: 2vw;
    }
}

@media screen and (width: 1024px) {
    .hero-img1 {
        position: relative;
        left: 10vw;
    }

    .hero-img2 {
        position: relative;
        left: -5vw;
    }

    .services {
        display: grid;
        grid-template-columns: repeat(2, 274.5px);
        gap: 5vw;
        margin: 5vh 10vw 2vh 20vw;

    }

    .support {
        grid-template-columns: 30vw 60vw;
        gap: 10vh;
    }

    .support div {
        margin-top: 0;
    }

    .support img {
        margin-left: 0vw;
    }

}

@media screen and (min-width: 721px) and (max-width: 912px) {
    a {
        font-size: 18px;
    }

    .hero h1 {
        font-size: 64px;
        line-height: 70.14px;
    }

    .menu {
        display: none;
    }

    .hero button {
        width: 342px;
        padding-top: 1.5vh;
        padding-bottom: 1.5vh;
    }

    .hero-images {
        display: flex;
    }

    .hero-img1 {
        position: relative;
        left: 3vw;
    }

    .hero-img2 {
        position: relative;
        right: 18vw;
    }


    .services {
        display: grid;
        grid-template-columns: repeat(2, 274.5px);
        gap: 2vw;
        margin: 5vh 10vw 2vh 13vw;

    }

    .services_info img {
        margin: 5vh 2vw 0 2vw;
    }

    .services_info h3 {
        margin: 2vh 2vw 0 2vw;
        color: #1B1D21;
    }

    .service-discription {
        padding-top: 5vh;
    }

    .service-discription h1 {
        font-weight: 700;
        font-size: 40px;
    }

    .signUp {
        padding: 10vh 10vw 10vh 10vw;
        display: grid;
        grid-template-columns: 31vw 40vw;
        gap: 10vw;
    }

    .min-signup {
        margin-top: 0;
    }

    .min-signup ul li {
        margin: 0;
        margin-bottom: 3vh;
        padding: 0;
        display: grid;
        grid-template-columns: 2vw 25vw;
        gap: 5vw;
    }

    .min-signup h1 {
        color: #131313;
        font-size: 40px;
        font-weight: 700;
    }

    .min-signup button {
        width: 30vw;
        margin-left: 0;
        padding-top: 1.5vh;
        padding-bottom: 1.5vh;
    }

    .mainh1 {
        font-size: 40px;
    }

    .support {
        background-image: url('../assest/images/home/background.png');
        background-color: #276E59;
        background-repeat: no-repeat;
        background-size: cover;
        display: grid;
        gap: 5vh;
        padding: 0vh 10vw 10vh 10vw;
    }

    .support button {
        width: 40vw;
        padding-top: 1vh;
        padding-bottom: 1vh;
        font-size: 14px;
    }

    .support img {
        margin-left: 10vw;
    }



    .newsletter {
        top: 15vh;
    }

    .newsletter-signup {
        margin: 3vh 0 5vh 0;
    }

    .newsletter-signup button {
        padding-top: 1.5vh;
        padding-bottom: 1.5vh;
        width: 25vw;
    }

    .newsletter-signup input {
        padding: 0 0 0 2vw;
    }

    .newsletter-details h1 {
        font-size: 30px;
        line-height: 40px;
    }

    footer {
        padding-top: 20vh;
        grid-template-columns: 40vw 22vw 25vw;
    }

    .contactus ul li {
        grid-template-columns: 2vw 20vw;
        gap: 2vw;
    }



}

@media only screen and (min-width: 481px) and (max-width: 720px) {
    nav .logoul {
        padding: 0;
    }

    .navbar {
        margin-top: 1vh;
    }

    .hero h1 {
        font-size: 54px;
        line-height: 70.14px;
    }

    .hero button {
        width: 342px;
    }

    .hero-images {
        display: flex;
    }

    .hero-img1 {
        width: 50vw;
        left: 0;
    }

    .hero-img2 {
        position: relative;
        width: 50vw;
        right: 20vw;
    }


    .services {
        display: grid;
        gap: 5vw;
        grid-template-columns: repeat(2, 200px);
        margin: 5vh 10vw 2vh 10vw;
    }

    .services_info {
        height: 200px;
        background-color: #FFFFFF;
        text-align: left;
    }


    .services_info img {
        margin-top: 4vh;
    }

    .services_info h3 {
        margin: 2vh 2vw 0 2vw;
        color: #1B1D21;
    }

    .service-discription {
        padding-top: 5vh;
    }

    .service-discription h1 {
        font-weight: 700;
        font-size: 40px;
    }

    .signUp {
        padding: 10vh 10vw 10vh 10vw;
        display: grid;
        gap: 0;
    }

    .signUp .iphone {
        margin-left: 12vw;
    }

    .min-signup ul li {
        margin: 0;
        margin-bottom: 5vh;
        padding: 0;
        display: grid;
        grid-template-columns: 10vw 70vw;
        gap: 2vw;
    }

    .min-signup h1 {
        color: #131313;
        font-size: 40px;
        font-weight: 700;
    }

    .min-signup button {
        width: 40vw;
        margin: 0;
    }

    .support {
        background-image: url('../assest/images/home/background.png');
        background-color: #276E59;
        background-repeat: no-repeat;
        background-size: cover;
        display: grid;
        gap: 5vh;
        padding: 0vh 10vw 10vh 10vw;
    }

    .support button {
        width: 40vw;
    }

    .newsletter {
        position: static;
        margin: 5vh 5vw 5vh 5vw;
        display: grid;
        grid-template-rows: 30vw 40vw;
        grid-template-columns: none;
    }

    .newsletter-details h1 {
        font-size: 35px;
        line-height: 40px;
    }

    .newsletter-signup input {
        padding-left: 5vw;
        font-size: 20px;
    }

    .newsletter-signup button {
        width: 80vw;
        font-size: 20px;
    }

    footer {
        background-color: #0B0D17;
        color: #FEFEFE;
        display: grid;
        gap: 2vw;
        margin: 0;
        grid-template-rows: 30vw 18vw 38vw;
        grid-template-columns: none;
        padding: 10vw 5vw 10vw 5vw;

    }

    .socials ul {
        gap: 10vw;
    }

    .socials ul img {
        width: 4vw;
    }

    .logo2 {
        width: 25vw;
    }

    .links h1 {
        font-size: 30px;
    }

    .links ul {
        display: flex;
        gap: 4vw;
    }

    .links ul li a {
        font-size: 18px;
    }


    .contactus h1 {
        font-size: 30px;
    }

    .contactus ul li {
        display: grid;
        grid-template-columns: 2vw 60vw;
        gap: 5vw;
        margin-bottom: 2vh;
    }


    .contactus ul li p {
        color: #D9DBE1;
        font-weight: 400;
        font-size: 18px;
    }


}

@media screen and (width: 1440px) {
    .hero button {
        font-size: 18px;
        padding-top: 1.5vw;
        padding-bottom: 1.5vw;
    }

    .hero-img1 {
        left: 18vw;
    }

    .hero-img2 {
        left: 6vw;
    }
}

@media screen and (min-width: 1440px) {
    .hero-img2 {
        left: 8vw;
    }
}

@media screen and (width:2560px) {
    .hero p {
        font-size: 30px;
        line-height: 40px;
    }

    .hero-img1 {
        position: relative;
        left: 25vw;
    }

    .hero-img2 {
        position: relative;
        right: 0vw;
        left: 20vw;
    }

    .hero button {
        font-size: 20px;
    }

    .service-discription h1 {
        font-size: 50px;
    }

    .service-discription p {
        font-size: 30px;
    }

    .services {
        margin-left: 25vw;
    }

    .services_info h3 {
        font-size: 30px;
    }


}

@media only screen and (max-width:480px) {

    .close,
    .menu {
        display: block;
        position: absolute;

    }

    .close {
        z-index: 2;
        top: 5vh;
        left: 80vw;
        display: none;
        position: fixed;
    }

    .menu {
        left: 80vw;
    }

    .logoul {
        padding: 0;
    }

    .logo {
        width: 30vw;
        margin: 0;
    }

    .navbar {
        position: absolute;
        position: fixed;
        top: 0;
        left: 35vw;
        background-color: #FFFFFF;
        color: #276E59;
        height: 101vh;
        display: grid;
        grid-template-rows: 10vh 10vh 10vh 10vh;
        width: 55vw;
        z-index: 1;
        padding-top: 20vh;
        display: none;
    }

    .navbar li {
        display: block;
        margin-bottom: 5vh;
    }

    .navbar li a {
        color: #276E59;
        text-decoration: none;
        font-size: 20px;
        cursor: pointer;
    }

    .navbar a.router-link-active {
        color: #276E59;
        text-decoration: none;
    }

    .hero h1 {
        font-size: 44px;
        line-height: 50.14px;
    }

    .hero button {
        width: 300px;
    }

    .hero-images {
        display: flex;
    }

    .hero-img1 {
        width: 50vw;
        left: 0;
    }

    .hero-img2 {
        position: relative;
        width: 50vw;
        right: 25vw;
    }

    .services {
        display: grid;
        gap: 5vw;
        grid-template-columns: repeat(2, 150px);
        margin: 5vh 10vw 2vh 8vw;
    }


    .services_info {
        height: 150px;
        background-color: #FFFFFF;
        text-align: left;
    }

    .services_info img {
        margin: 2vh 2vw 0 3vw;
        width: 15vw;
    }

    .services_info h3 {
        margin: 2vh 2vw 0 3vw;
        font-size: 16px;
        width: 100%;
        color: #1B1D21;
    }

    .service-discription {
        padding-top: 10vh;
    }

    .service-discription h1 {

        font-weight: 700;
        font-size: 30px;
    }

    .service-discription p {
        padding: 0 5vw 0 5vw;
    }

    .signUp {
        padding: 10vh 10vw 10vh 8vw;
        display: grid;
        gap: 0;
    }

    .signUp .iphone {
        position: relative;
        left: 18vw;
        width: 50vw;

    }

    .min-signup {
        margin-top: 5vh;
    }

    .min-signup h1 {
        color: #131313;
        font-size: 30px;
        font-weight: 700;
        text-align: center;
        margin: 0;
    }

    .min-signup ul {
        margin-bottom: 5vh;
    }

    .min-signup ul li {
        margin: 0;
        margin-bottom: 2vh;
        padding: 0;
        display: grid;
        grid-template-columns: 10vw 70vw;
        gap: 5vw;
    }

    .min-signup button {
        width: 75vw;
    }

    .mainh1 {
        font-size: 30px;
    }

    .support {
        background-image: url('../assest/images/home/background.png');
        background-color: #276E59;
        background-repeat: no-repeat;
        background-size: cover;
        display: grid;
        gap: 5vh;
        padding: 0vh 10vw 10vh 10vw;
    }

    .support img {
        width: 70vw;
        margin-left: 5vw;
    }

    .support button {
        width: 70vw;
        font-size: 16px;
    }

    .newsletter {
        position: static;
        margin: 5vh 5vw 5vh 5vw;
        display: grid;
        grid-template-rows: 50vw 50vw;
        grid-template-columns: none;
    }

    .newsletter-details h1 {
        font-size: 30px;
        font-weight: 700px;
        line-height: 40px;
    }

    .newsletter-signup input {
        padding-left: 10vw;
    }


    .newsletter-signup button {
        width: 80vw;

    }

    footer {
        background-color: #0B0D17;
        color: #FEFEFE;
        display: grid;
        gap: 10vw;
        margin: 0;
        grid-template-rows: 30vw 25vw 50vw;
        grid-template-columns: none;
        padding: 10vw 5vw 10vw 5vw;

    }

    .socials ul {
        gap: 20vw;
    }


    .logo2 {
        width: 20vw;
    }

    .links ul {
        display: flex;
        gap: 4vw;
    }

    .contactus ul li {
        display: grid;
        grid-template-columns: 2vw 60vw;
        gap: 5vw;
        margin-bottom: 2vh;
    }


    .contactus p {
        color: #D9DBE1;
        font-weight: 400;
        font-size: 14px;
    }


}

@media  screen and (width:425px) {
    .services {
        margin: 5vh 10vw 2vh 10vw;
    }
}

@media only screen and (min-width:280px) and (max-width:320px) {
    .hero h1 {
        font-size: 30px;
        line-height: 30px;
    }

    .hero button {
        width: 200px;
    }

    .services {
        display: grid;
        gap: 5vw;
        grid-template-columns: repeat(2, 100px);
        margin: 5vh 10vw 2vh 10vw;
    }

    .service-discription h1 {
        font-size: 20px;
    }

    .service-discription p {
        font-size: 14px;
        padding-left: 2vw;
        padding-right: 2vw;
    }

    .services_info {
        height: 100px;
    }

    .services_info h3 {
        font-size: 11px;
    }

    .newsletter {
        gap: 15vh;
    }

    .newsletter-details h1 {
        font-size: 30px;
    }

    .newsletter-signup input {
        height: 40px;
    }

    footer {
        gap: 10vh;
        padding-top: 10vh;
        padding-bottom: 10vh;
    }

    .socials .logo2 {
        width: 40vw;
    }

}</style>
