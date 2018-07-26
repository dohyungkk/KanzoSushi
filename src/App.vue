
<template>

<div id="app">


  <div id="header">
    <h1 id="headerTitle">
       <div id='logo'>
        <img class="imageAboutUs" src="./assets/kanzoLogo-1.jpg"></img>
      </div>
        <div id="buttonGrouped">
      <b v-scroll-to="'#home'">Home</b>
      <b v-scroll-to="'#about'">About</b>
      <b v-scroll-to="'#comment'">Comment</b>
      <b v-scroll-to="'#menu'">Menu</b>
      <b v-scroll-to="'#gallery'">Gallery</b>
      <b v-scroll-to="'#contact'">Contact Us</b>

    </div>

    </h1>



  </div>


    <div id='home'><Intro/></div>
    <div id='about'><AboutUs/></div>
    <div id='comment'><CustomerComment/></div>
    <div id='menu'><Menu/></div>
    <div id='gallery'><Gallery/></div>
    <div id='contact'><FooterBar/></div>

  </div>
</template>

<script>

document.title = "Kanzo Sushi"
import Intro from './components/Intro'
import AboutUs from './components/AboutUs'
import CustomerComment from './components/CustomerComment'
import Menu from './components/Menu'
import Gallery from './components/Gallery'
import FooterBar from './components/FooterBar'

export default {
  name: 'app',
  components: {
    Intro,AboutUs,CustomerComment,Menu,Gallery,FooterBar
  },

}


</script>

<style>

html {
  width: 100%; height: 100%;
}

body {
  margin: 0px; padding: 0px;
  font: 14px serif;
  width: 100%; height: 100%;
}

h1 {
  margin: 0px;
  padding: 30px 0px;
  color: #CCC;
  font: bold 40px serif;
  letter-spacing: 5px;
  text-align: left;
}

p {
  margin: 0px;
  padding: 10px 20px;
  line-height: 1.5;
}



b {
  font-size: 20px;
}
#header {
  margin-bottom: 0px;
  padding-top: 0px;
  position: relative;
  background: black;
  width: 100%; height: 100%;
}

#logo {
  height: 100px;
  font-size: 30px;
  margin: 0 60px 0 0;

}

.buttonGrouped {
  float:right;
}

#buttonGrouped b:hover {
  background: red;
  background: linear-gradient(#222, #333);
}

#content {
  margin: 0px;
  padding: 0px 0px 0px 0px;
}

#headerTitle {
  text-align: center;
}

img {
    vertical-align: left;
    border-style: none;
}

</style>
