<template>
  <div class="home">
    <Carousel />
  </div>
</template>

<script>
import Carousel from '@/components/Carousel.vue';

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Home',
  components: {
    Carousel
  }
}
</script>
