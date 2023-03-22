<template>
  <div class="container">
    <div class="header">
      <nav>
        <ul class="logoul">
          <li><router-link to="/"><img src="../assest/images/home/Logo.png" alt="Company Logo" class="logo"></router-link>
          </li>
          <li>
            <img src="../assest/images/icon-menu-close.svg" alt="" class="close" ref="close" @click="close">
            <img src="../assest/images/icon-menu.svg" alt="" class="menu" ref="menu" @click="open">
          </li>
          <li>
            <ul class="navbar" ref="navbar">
              <li><router-link to="/">Home</router-link></li>
              <li><router-link to="#">About</router-link></li>
              <li><router-link to="/business">For Business</router-link></li>
              <li><router-link to="/faq">FAQs</router-link></li>
            </ul>
          </li>
        </ul>
      </nav>
    </div>

    <main>

      <div class="accordion">
        <div v-for="(item, id) in items">
        <h1><span>{{item.title}}</span> <img src="../assest/images/faq/arrowdown.png" @click="toggle"  alt=""></h1>
        <hr>
        <p>{{ item.content }}</p>
        </div>
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
        <li><a href="https://www.instagram.com/dexterapp_hq/"><img src="../assest/images/home/instagram.png" alt=""></a>
        </li>
        <li><a href="https://www.linkedin.com/company/dexterapphq/"><img src="../assest/images/home/twitter.png"
              alt=""></a></li>
        <!-- <li><a href="https://www.tiktok.com/@dexter_app"><img src="../assest/images/home/tiktok-logos-ideLwxpXwt.png" alt=""></a></li> -->
        <li><a href="#"><img src="../assest/images/home/linkedin.png" alt=""></a></li>
      </ul>
    </div>
    <div class="links">
      <h1>Quick Links</h1>
      <ul>
        <li><router-link to="#">About</router-link></li>
        <li><router-link to="#">Contact</router-link> </li>
        <li><router-link to="/faq">FAQs</router-link> </li>
        <li><router-link to="/termOfServices">Term Of Service</router-link> </li>
        <!-- <li><router-link to="/ImageCredits">Image Credits</router-link></li> -->
      </ul>
    </div>
    <div class="contactus">
      <h1>Contact</h1>
      <ul>
        <li><img src="../assest/images/home/mail.png" alt="">
          <p>support@dexterapp.com</p>
        </li>
        <li><img src="../assest/images/home/tel.png" alt="">
          <p>+234 703 231 9537</p>
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
      items: {
        first: {
          title: 'What is DexterApp?',
          content: 'Dexter app is a platform that connects customers with a network of skilled vendors offering various technical services. Whether you need a plumber, electrician, or handyman, Dexter app makes it easy to find and hire the right professional for the job. With transparent pricing and easy scheduling, Dexter app takes the hassle out of finding reliable service providers.'
        },
        second: {
          title: 'How can I use DexterApp as a customer?',
          content: 'Visit getdexterapp.com or download the customer app on Playstore/Appstore @DexterApp. Sign in if you are a registered user or Create an Account here. Browse through a wide range of our services and pick any of your choice.'
        },
        third: {
          title: 'How can I use Dexter Vendor App?',
          content: 'Visit getdexterapp.com or download the Vendor app on Playstore/Appstore @DexterApp. Sign in if you are a registered user or Create an Account here. Browse through a wide range of our services and pick any of the service you offer.'
        },
        fourth: {
          title: 'Is DexterApp free to use?',
          content: 'Yes DexterApp is absolutely free to use'
        },
        fifth: {
          title: 'How do I report a scam case?',
          content: 'In a scam or if you have suspicions that one of our users may deceive people, please tell us about it via email @ support@dexterapp.com Share a link to the profile of such a user and describe all the details you have. Attach screenshots of your conversations and other pictures or materials that can give us more information in taking the necessary steps.'
        }
      }
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
    },
    toggle() {
      this.img = '../assest/images/faq/arrowup.png'
      console.log(this.img)
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

.accordion {
  margin: 0;
  padding: 10vh 10vw 0vh 12vw;

}

.accordion div {
  border: 1px solid #999999;
  border-radius: 15px;
  padding: 10px;
  margin-bottom: 5vh;
}

.accordion h1 {
  margin: 0;
  font-size: 16px;
}

.accordion h1 img {
  float: right;
}

.accordion p {
  color: #999999;
  font-size: 14px;
}


.newsletter {
  position: relative;
  background-color: #276E59;
  display: grid;
  grid-template-columns: 40vw 20vw;
  margin: 0 vh 10vw 0vh 10vw;
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

@media screen and (width: 1024px) {}

@media screen and (min-width: 721px) and (max-width: 912px) {
  a {
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

@media only screen and (min-width: 481px) and (max-width: 720px) {
  nav .logoul {
    padding: 0;
  }

  .navbar {
    margin-top: 1vh;
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

@media screen and (width: 1440px) {}

@media screen and (min-width: 1440px) {}

@media screen and (width:2560px) {}

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

@media screen and (width:425px) {}

@media only screen and (min-width:280px) and (max-width:320px) {
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

}
</style>
