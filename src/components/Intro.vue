<template>
  <div>
    <div v-for="number in [currentNumber]" transition="fade">
    <img class='images' :src="images[currentNumber % images.length]  " />
    </div>
  </div>
</template>



<script>
export default {
  data () {
    return {
       images: [require('../assets/DSC00284.jpg'), require('../assets/DSC00161.jpg'), require('../assets/DSC00122.jpg')],
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

  div {
    padding: 0;
    margin: 0;
  }

  a {
     font-family:  serif;
  }

  .images {
    height: 100%;
    width: 100%;
  }

.fade-transition {
  transition: all 0.8s ease;
  overflow: hidden;
  visibility: visible;
  opacity: 1;
  position: relative;
}
.fade-enter, .fade-leave {
  opacity: 0;
  visibility: hidden;
}

</style>


