<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <router-view/>
  </div>
</template>

<style>
@import url("https://fonts.googleapis.com/css?family=Roboto:300,400,500,700");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
:root{
  --white: #ffffff;
  --grey: #414141;
  --red: 	#d62d20;
  --amarillo: #ffa700;
  --blue:#9e0000;
  --orange:#e34c26;
  --green:#008744;
  --blueReact: #61DBFB;
}

a {
  text-decoration: none;
  color: var(--white);
}

a:hover {
  color: #bbbbbb;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: "Roboto", sans-serif;
  background:var(--white);
  color: #f5f5f5;
}

section {
  padding: 90px 0;
  text-align: center;
  background: white;
}

.container {
  width: 100%;
  display: inherit;
  max-width: 1200px;
  justify-content: inherit;
  margin: 0 auto;
  padding: 0 20px;
}

.navbar {
  position: fixed;
  /* background: transparent; */
  background-color: #000000ca;
  transition: background 0.3s;
  display: flex;
  justify-content: space-between;
  height: 60px;
  width: 100%;
  z-index: 5;
}

.navbar__logo {
  display: flex;
  align-items: center;
}

.navbar__title {
  font-size: 24px;
}

.navbar__title::before {
  content: "<";
  color:var(--blue);
}

.navbar__title::after {
  content: "/>";
  color: var(--blue);
}

.navbar__links {
  list-style: none;
  display: flex;
  height: 100%;
  align-items: center;
}

.navbar__link {
  padding-left: 20px;
}

.navbar__link a {
  color: #8e8e8e;
  transition: color 0.3s;
}

.navbar__link a:hover {
  color: var(--blue);
  transition: color 0.3s;
}

.navbar__menu {
  display: none;
  align-items: center;
  font-size: 35px;
}

.home {
  min-height: 100vh;
  display: flex;
  padding: 30px;
  justify-content: center;
  align-items: center;
  background: rgba(0, 0, 0, 0.8);
  position: relative;
}

.home__background {
  background-color: #8e8e8e;
  background-image: url(./assets/img/bg.webp);
  background-attachment: fixed;
  background-size: cover;
  background-position: center;
  height: 100%;
  width: 100%;
  position: absolute;
  z-index: -1;
}

.home__profile {
  height: 250px;
  border-radius: 50%;
  margin-right: 40px;
  transition: filter  3s;
}
.coder-img{
  height: 400px;
  margin-left: 50px;
  transition: filter  3s;
}
.midiom{
  margin: 0;
}
.home__title {
  font-size: 60px;
  text-shadow: 1px 1px black;
  color: var(--blue);
}
.home__description{
  width: 50%;
}

.home__title--primary,
.home__title--secondary {
  font-size: 25px;
  color: #f5f5f5;
  text-shadow: 1px 1px black;
}


.section__title {
  color: var(--grey);
  font-size: 35px;
  margin-bottom: 30px;
  display: flex;
}

.section__subtitle {
  color: var(--grey);
  text-align: start;
  margin-bottom: 20px;
}

.about__grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 20px;
}

.about__description {
  text-align: left;
  color: var(--grey);
  /* padding-right: 80px; */
  line-height: 30px;
}

.about__summary {
  margin: 30px 0;
}

.about__description span {
  color: var(--grey);
}

.about__description h2 {
  color: var(--grey);
  margin: 20px 0;
}

.about__skills {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 10px;
}

.skill__title {
  color: var(--grey);
  grid-column: span 3;
  text-align: left;
  margin: 20px 0;
}

.skill__item {
  font-size: 65px;
  color: var(--grey);
  padding: 35px;
  transition: all 0.3s;
  min-width: 130px;
  height: 180px;
}
.fa-html5{
  color: #e34c26;
}

.fa-css3-alt{
  color: #264de4;
}

.fa-js{
  color:#f0db4f ;
}

.fa-git-alt{
  color: #f34f29;
}

.fa-react{
  color: var(--blueReact);
}


.skill__name {
  font-size: 16px;
  text-align: center;
}

.services__grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 20px;
}

.services__item {
  padding: 20px;
  /* background: rgba(245,245,245,0.6); */
  border-bottom: 5px solid transparent;
  border-radius: 10px;
  transition: border 0.3s;
}

/* .services__item:hover {
  transition: border 0.3s;
  border-bottom: 5px solid var(--blue);
} */

.services__item:hover i {
  transition: all 0.3s;
  color: var(--grey);
}

.services__item i {
  transition: all 0.3s;
  font-size: 40px;
  margin: 20px 0;
}

.fa-mobile-alt{
  color: black;
}

.fa-pencil-ruler{
  color: var(--orange);
}

.fa-code{
  color: var(--green);
}

.fa-thumbs-up{
  color: var(--red);
}

.fa-tachometer-alt{
  color: var(--amarillo);
}

.fa-crosshairs{
  color: var(--blue);
}

.services__item h3 {
  color: var(--grey);
  margin-bottom: 15px;
}

.services__item p {
  color: var(--grey);
}

.team__grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  gap: 20px;
}

.team__item {
  background: white;
  position: relative;
  object-fit: cover;
  overflow: hidden;
  font-size: 14px;
  border-radius: 10px;
  /* background-color: #008744; */
  width: 100%;
  /* height: 500px; */
}

.team__img {
  width: 100%;
  height: 100%;

  object-fit: cover;
  display: block;
  transition: all 1s;
  border-radius: 10px;
  /* max-height: 190px; */
}

.team__description {
  padding: 50px;
  position: absolute;
  background-color: rgba(0, 0, 0, 0.7);
  top: 300px;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: all 0.5s;
  border-radius: 10px;
  z-index: 1;
  display: flex;
  justify-content: center;
  flex-direction: column;
}

.team__item:hover .team__description {
  visibility: visible;
  opacity: 1;
  transition: all 0.5s;
  border-radius: 10px;
  transform: translateY(-300px);
}

.team__item:hover .team__img {
  transition: all 1s;
  border-radius: 10px;
  /* transform: scale(1.3); */
}

.team__description--title {
  color: var(--white);
}

.team__description--text {
  margin: 20px 0;
}

.buttons__container {
  display: flex;
  border-radius: 10px;
}

.button {
  background: #191919;
  color: #f5f5f5;
  padding: 5px 10px;
  display: inline-block;
  margin: auto;
}

.button:hover {
  color: var(--blue);
}




.button--cta {

  background: var(--blue);
  color: var(--white);
  padding: 5px 30px;
  display: inline-block;
  align-self: center;
  margin: 20px auto;
  font: bold;
  border-radius: 5px;
}

.button--cta i {
  margin-right: 10px;
}

.button--cta:hover {
  background: var(--grey);
  color: white;
}

.contact__grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  gap: 30px;
}

.contact__item {
  color: var(--grey);
  padding: 40px;
  transition: all 0.3s;
}

.fa-envelope{
  color: var(--red);
}

.fa-github{
  color: black;
}

.fa-twitter{
  color: #00acee;
}

.fa-linkedin-in{
  color:#0e76a8  ;
}

.contact__item i {
  font-size: 50px;
  margin-bottom: 10px;
}

.fa-envelope:hover {
  transition: all 0.3s;
  color: var(--grey);
}
.fa-github:hover {
  transition: all 0.3s;
  color: var(--grey);
}
.fa-twitter:hover {
  transition: all 0.3s;
  color: var(--grey);
}
.fa-linkedin-in:hover {
  transition: all 0.3s;
  color: var(--grey);
}
/* .active a {
  color: #f5f5f5;
} */

.footer {
  color: var(--grey);
  background-color: rgba(245,245,245,0.6);
  padding: 30px;
  text-align: center;
  font-size: 14px;
}

.footer a {
  color: var(--grey);
}

.footer a:hover {
  color: var(--blue);
}

@media (max-width: 991px) {



  .navbar__menu {
    display: flex;
  }

  .navbar__links {
    position: absolute;
    width: 100vw;
    height: 100vh;
    flex-direction: column;
    background: rgba(0, 0, 0, 0.97);
    font-size: 30px;
    margin: 0 -20px;
    z-index: 10;
    transform: translateX(100%);
    opacity: 0;
    transition: all 0.5s;
  }

  .visible {
    display: flex;
    transform: translateX(0);
    opacity: 1;
    transition: all 0.5s;
  }

  .navbar__link {
    padding-left: 0px;
    margin-top: 30px;
  }

  section {
    padding: 50px 0;
  }

  .home {
    flex-direction: column;
  }

  .home__profile {
    margin-bottom: 30px;
    margin-right: 0;
  }

  .home__title {
    font-size: 45px;
  }

  .home__title--primary,
  .home__title--secondary {
    font-size: 20px;
  }

  .section__title {
    font-size: 25px;
  }

  .section__title:after {
    width: 110px;
    height: 3px;
  }

  .section__subtitle {
    
    font-weight: normal;
  }

  .about__description {
    padding-right: 0px;
  }

  .about__grid {
    grid-template-columns: 1fr;
  }

  .skill__title {
    grid-column: span 4;
  }

  .about__skills {
    grid-template-columns: 1fr 1fr 1fr 1fr;
  }

  .button--cta {
    margin-bottom: 30px;
  }

  .services__item {
    padding: 15px;
  }

  .services__item h3 {
    margin-bottom: 5px;
  }

  .services__grid,
  .team__grid {
    grid-template-columns: 1fr 1fr;
    gap: 20px;
  }
}

@media (max-width: 767px) {

  
  .home__background {
    background-image: url(./assets/img/bg_responsive.webp);
    background-attachment: fixed;
    background-size: cover;
    background-position: center;
  }

  section {
    padding: 20px 0;
  }

  .home__profile {
    margin-bottom: 30px;
  }

  .home__title {
    font-size: 30px;
  }

  .home__title--primary,
  .home__title--secondary {
    font-size: 20px;
  }

  .skill__title {
    grid-column: span 3;
  }

  .about__skills {
    grid-template-columns: 1fr 1fr 1fr;
  }

  .skill__item {
    font-size: 50px;
    padding: 5px;
    min-width: 75px;
    height: 85px;
  }

  .services__grid,
  .team__grid {
    grid-template-columns: 1fr;
    gap: 20px;
  }


  .contact__grid {
    grid-template-columns: 1fr 1fr;
  }

  .contact__item {
    padding: 18px;
    border-radius: 10px;
    transition: all 0.3s;
  }
}
</style>