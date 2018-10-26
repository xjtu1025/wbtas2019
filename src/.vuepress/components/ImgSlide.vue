<template>
  <Carousel :perPage="1" :loop="true" :autoplay="true" :autoplayTimeout="3000">
    <Slide v-for="img in imgs" :key="img">
      <img :src="img"/>
    </Slide>
  </Carousel>
</template>

<script>
import { Carousel, Slide } from '../../../node_modules/vue-carousel'

export default {
  name: 'ImgSlide',

  components: {
    Carousel,
    Slide
  },
  
  data () {
    return {
      imgs: [
        'https://saner2019.github.io/img_system/ZJU-overview-words-white.jpeg',
        'https://saner2019.github.io/img_system/002-wods.jpeg',
        'https://saner2019.github.io/img_system/003-words.jpg',
      ]
    }
  },
}
</script>
