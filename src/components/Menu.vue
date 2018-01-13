<template>
  <div>
    <div class="backgroundMenuImage">
      <div class="catchyTitle"> Menu</div>
      <hr>
        <body>
           <div>
    <gallery :images="images" :index="index" @close="index = null"></gallery>

    <div class='wrapper'>
    <div
      class="image"
      v-for="(image, imageIndex) in images"
      :key="imageIndex"
      @click="index = imageIndex"
      :style="{ backgroundImage: 'url(' + image + ')', width: '300px', height: '200px' }"
    ><img class='images' :src="images[currentNumber % images.length]  " /></div>
  </div>
  </div>

        </body>
   </div>
 </div>
</template>

<script>
import VueGallery from './slider/gallery';

export default {
    data: function () {
      return {
        images: [
          // require('../assets/DSC00012-2.jpg'),
          // require('../assets/DSC00031.jpg'),
          // require('../assets/DSC00092.jpg'),
          // require('../assets/DSC00094.jpg'),
          // require('../assets/DSC00149.jpg'),
          require('../assets/menu1.jpg'),
          require('../assets/menu2.jpg')
        ],
        index: null
      };
    },

    components: {
      'gallery': VueGallery
    },
  }

</script>


<style scoped>

  .body {
    size: 100%;
  }


  .backgroundMenuImage {
    height: 100%;
    width: 100%;
    background-color: white;
  }

   .catchyTitle {
    color: #CD594A;
    padding-top: 30px;
    text-align: left;
    font-size: 50px;
  }

   .image {
    position: relative;
    display: inline-block;
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;
    border: 1px solid #ebebeb;
    margin: 5px;
    height: 50%;
  }

</style>
