<template>
  <div>
    <div class="backgroundAboutUsImage">
      <div class="catchyTitle"> ͏Ab͏o͏u͏t ͏Us</div>
      <hr>
        <div class="descriptionBox">
        <p class="descriptionTitle"> Kanzo's Story</p>
        <p class="descriptionDetail"> Kanzo Sushi is a fun and welcoming place to enjoy simple, fresh and delicious sushi crafted using a combination of Japanese ingredients and fresh products. <br /><br /> Come for takeouts! </p>
        </div>
        <div class="descriptonBox2">
          <img class='images' :src="images[currentNumber % images.length]  " />
        </div>
    </div>

<!-- TODO for Kevin: a) Pictures while rotating breaks out of the DOM. Check the rotation and adjust css. b) Is it neccesary to make this picture rorate? Seems like it's only piling up the runtime and is not neccesary. As mentioned in other TODO, if you can compress the pic, then this would be viable but if not, just get rid of multiple picture rotation for runtime's sake. -->

  </div>
</template>

<script>
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

export default {
  data () {
    return {
       images: [require('../assets/2.jpg'), require('../assets/3.jpg'), require('../assets/4.jpg'), require('../assets/5.jpg'), require('../assets/6.jpg'), require('../assets/7.jpg')],
        currentNumber: 0
    }
  },
  beforeMount()  {
        this.startRotation();
    },

    methods: {
        startRotation: function() {
            this.timer = setInterval(this.next, 6000);
            console.log('rotation happens')
        },

        stopRotation: function() {
            clearTimeout(this.timer);
            this.timer = null;
        },

         next: function() {
            this.currentNumber += 1
        }

    }
}
</script>


<style scoped>

  p {
    margin-top: 0;
    margin-bottom: 1rem;
  }
  .descriptionBox {
    margin-top: 20px;
    padding-right: 100px;
    float: left;
  }

  .imageAboutUs {
    margin-top: 20px;
    float:right;
    height: 300px;
    width: 300px;
    margin-right: 150px;
  }

  .descriptionBox2 {
    margin-right: 150px;
  }

  .descriptionTitle {
    font-size: 30px;
    font-weight: bold;

  }

  .descriptionDetail {
    font-size: 15px;
    font-style: italic;
    width: 500px;


  }

  .backgroundAboutUsImage {
  height: 500px;
  opacity: 1;
  /*background: url("../assets/aboutusback.jpg") no-repeat center center fixed;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;*/
background-color: #FFF;
  }

  .catchyTitle {
    color: #CD594A;
    padding-top: 30px;
    text-align: left;
    font-size: 50px;

  }

  .images {
    height: 25%;
    width: 25%;
  }

@media all and (max-width: 1024px) and (min-width: 568px){
  .imageAboutUs {display:none; }
}




</style>


