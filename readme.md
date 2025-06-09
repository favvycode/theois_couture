<video autoplay muted loop playsinline>
  <source src="me.mp4" type="video/mp4">
</video>

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Theois_couture</title>
    <link rel="stylesheet" href="secondpage.css" />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Arimo:ital,wght@0,400..700;1,400..700&family=Josefin+Sans:ital,wght@0,100..700;1,100..700&family=Roboto:ital,wght@0,100..900;1,100..900&display=swap"
      rel="stylesheet"
    />
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css"
      integrity="sha512-Evv84Mr4kqVGRNSgIGL/F/aIDqQb7xQ2vcrdIwxfjThSH8CSR7PBEakCr51Ck+w+/U6swU2Im1vVX0SVk9ABhg=="
      crossorigin="anonymous"
      referrerpolicy="no-referrer"
    />
  </head>
  <body>
    <div class="content">
      <div class="section1">
        <input type="checkbox" id="menu-toggle" />
        <nav>
          <label for="menu-toggle" class="hamburger-icon"
        ><i class="fa-solid fa-bars"></i> <div id="mars-icon"><i class="fa-solid fa-xmark" ></i
      ></div></label>
      <div class="logo"><img src="./assert/images/logo.jpg" alt="logo" />Theois_couture</div>
    </nav>
    <div class="mobile-nav">
      <ul>
        <li ><a href="index.html" class="mobile-link-items">HOME</a></li>
        <li > <a href="infopage.html" class="mobile-link-items">INFO</a></li>
        <li > <a href="gallerypage.html" class="mobile-link-items">GALLERY</a></li>
        <li > <a href="contactpage.html" class="mobile-link-items">CONTACT</a></li>
        <li > <a href="faqpage.html" class="mobile-link-items">FAQ</a></li>
      </ul>
    </div>
    <div class="banner-left-section">
      <ul>
        <div>WE</div>
        <div>PROMISE</div>
        <div>COMFORT.</div>
      </ul>
            <small>Fashion is the sketch of identity, stitched in style.
Every seam is a signature, every fabric a statement.</small>
    </div>
    <button class="button-element">
          SHOP NOW <img src="./assert/images/arrow.svg" alt="arrow" />
        </button>
        <div class="socialmedia">
  <a href="https://www.instagram.com/theois__couture?igsh=MWNuZzkyeGJkZThxMw%3D%3D&utm_source=qr" target="_blank"><i class="fab fa-instagram"></i></a>
  <a href="https://www.tiktok.com/@theois_couture?_t=ZM-8x2SUVO4Le1&_r=1" target="_blank"><i class="fab fa-tiktok"></i></a>
  <a href="mailto:d26796766@gmail.com"><i class="fas fa-envelope"></i></a>
        </div>
      </div>
      <div class="section2"><img src="assert/images/doubra.jpg" alt="doubra"></div>
    </div>



    
    <script>
  window.addEventListener('DOMContentLoaded', () => {
    if (window.location.hash === "#mars-icon") {
      document.getElementById("menu-toggle").checked = true;
    }
  });
    </script>
  </body>
</html>



* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Roboto", serif;
}


html, body {
    height: 100%;
}

 body {
  display: flex;
  align-items: center;
  margin: 0;
  padding: 0;
  background-image: url("assert/images/doubra.jpg");
  background-size: cover; /* Stretch to fill the screen */
  background-position: center; /* Center the image */
  background-repeat: no-repeat;
  font-family: sans-serif;
  color: white; 
  object-fit: contain;
  box-sizing: border-box;
}

.content {
  margin: 100px auto;
  border-radius: 10px;
  display: flex;
  justify-content: center;
 /* border: 1px solid red;*/
  border-radius: 10px;
   position: relative;
  overflow: hidden;
  
}

.section1{
    background-color: rgba(255, 255, 255, 0.8);
    width: 40%;
    color: black;
    /*border: 1px solid green;*/
    border-radius: 10px;
    display: flex;
    flex-direction: column;
   
}


nav {
  height: 50px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 5px;
/*border: 2px solid yellow;*/
}

.hamburger-icon {
  display: flex;
  font-size: 15px;
  color: black;
  padding-left: 5px;
  /*border: 1px solid purple;*/
  position: relative;
  z-index: 101;

}

#menu-toggle:checked+nav+.mobile-nav {
  display: flex;
}

#menu-toggle:checked+nav .hamburger-icon .fa-bars {
  display: none;
}

#menu-toggle:checked+nav .hamburger-icon .fa-xmark {
  display: flex !important;
  padding-left: 0px;
  margin-left: 5px;
  background-color: #333;
  color: burlywood;
  border-radius: 50%;
  border: 8px solid black;
}


#menu-toggle {
  display: none;
}

#menu-toggle:not(:checked) + #mars-icon {
  display: none;
}

#menu-toggle+nav .hamburger-icon .fa-xmark {
  display: none;
}

.mobile-nav {
  display: none;
  position: absolute;
  z-index: 100;
  object-fit: contain;
  width: 100%;
  height: 100%;
  box-sizing: border-box;
  background-color: black;
  box-shadow: 4px 2px 4px rgba(0, 0, 0, 1);
  padding-top: 30px;
  justify-content: center;
  align-items: center;
  border-radius: 10px;
}

.mobile-nav>ul {
  list-style-type: none;
  display: flex;
  gap: 5px;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  background-color: #333;
  width: 50%;
  height: 60%;
  border-radius: 10px;
}


.mobile-link-items {
  font-size: 20px;
  cursor: pointer;
  font-weight: 500;
  min-width: 24px;
  transition: 0.5s;
  color: burlywood;
}



.mobile-link-items:hover {
  color: #007bff;
  text-decoration: underline;
}

.logo{
    display: flex;
    font-family: 'Playfair Display';
    font-size: 13px;
    font-weight: 450;
}


.logo img {
  max-width: 10%;
}



.banner-left-section {
  display: flex;
  flex-direction: column;
  width: 100%;
  gap: 3px;
  /*border: 1px solid blue;*/
 padding: 20px 20px;
 margin-top: 20px;
}

.banner-left-section>small {
  font-weight: 400;
  font-size: 8px;
  line-height: 110%;
  color: black;
  width: 120px;
  display: flex;
}

.banner-left-section>ul {
  line-height: 120%;
  color: black;
  font-size: 20px;
  font-weight: 500;
}


.button-element {
  outline-style: none;
  border: 0;
  border: 2px solid burlywood;
  background-color: burlywood;
  color: black;
  font-weight: 400;
  font-size: 7px;
  width: 50px;
  height: 20px;
  border-radius: 3px;
  cursor: pointer;
  margin-bottom: 60px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 2px;
  margin-left: 20px;
}



.button-element:hover {
  background: burlywood;
  border: 2px solid burlywood;
}

.button-element img{
  max-width: 10%;
  
}

.socialmedia{
  margin-left: 10px ;
  margin-bottom: 5px;
}
.socialmedia a {
  color: #333;
  font-size: 20px;
  margin: 0px 10px;
  text-decoration: none;
}


.socialmedia a:hover {
  color: #007bff; 
}

.section2{
    background-color: rgba(0,0,0,0.5);
    height: auto;
    width: 40%;
    color: black;
    border: 1px solid black;
    border-radius: 10px;
    margin: 0;
  padding: 0;
  position: relative;
}

.section2 img{
  position: absolute;
  display: flex;
  object-fit: contain;
  height: 100%;
  max-width: 100%;
  object-fit: cover;
  border-radius: 10px;
}

@media (min-width :768px){
   .section1,
   .section2 {
    width: 45%;  
}

nav {
  height: 80px;
  gap: 10px;
}

.hamburger-icon {
  font-size: 25px;
  padding-left: 20px;
}

.logo{
    font-size: 20px;
    font-weight: 450;
}

.mobile-nav{
  padding-top: 60px;
}


.mobile-link-items {
  font-size: 25px;
}

.logo img {
  max-width: 8%;
}

.banner-left-section {
 padding: 20px 53px;
 gap: 10px;
 margin-top: 40px;
}

  .banner-left-section>small {
  font-weight: 500;
  font-size: 10px;
  width: 200px;
}

.banner-left-section>ul {
  font-size: 25px;
}

.button-element {
  font-size: 9px;
  width: 70px;
  height: 30px;
  margin-bottom: 90px;
  margin-left: 50px;

}

.socialmedia{
  margin-left: 40px ;
  margin-bottom: 5px;
}

.socialmedia a {
  font-size: 25px;
}

}

@media (min-width :1000px){
   .section1,
   .section2 {
    width: 50%;  
}

nav {
  height: 80px;
  gap: 10px;
}

.hamburger-icon {
  font-size: 25px;
  padding-left: 20px;
}

.logo{
    font-size: 25px;
    font-weight: 450;
}


.logo img {
  max-width: 8%;
}

.banner-left-section {
 padding: 50px 53px;
 gap: 10px;
 margin-top: 20px;
}

  .banner-left-section>small {
  font-weight: 500;
  font-size: 10px;
  width: 350px;
}

.banner-left-section>ul {
  font-size: 25px;
}

.button-element {
  font-size: 11px;
  width: 85px;
  height: 40px;
  margin-bottom: 70px;
  margin-left: 50px;

}

.socialmedia{
  margin-left: 40px ;
  margin-bottom: 5px;
}

.socialmedia a {
  font-size: 25px;
}

.mobile-nav{
  padding-top: 60px;
}


.mobile-link-items {
  font-size: 30px;
}
}