<template>
  <div id="app">
    <image-slider :images="images" :params="{minMoveDistance: 50, autoPlay: true}"></image-slider>
  </div>
</template>

<script>
import ImageSlider from './components/ImageSlider.vue'
import first from './assets/first.jpeg'
import sec from './assets/sec.jpeg'
import three from './assets/three.jpeg'
import four from './assets/four.jpeg'
import five from './assets/five.jpeg'

export default {
  name: 'app',
  components: {
    ImageSlider
  },
  data () {
    return {
      images: 
      [
        first,
        sec,
        three,
        four,
        five
      ]
    }
  }
}
</script>

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
</style>
