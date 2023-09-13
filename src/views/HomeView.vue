<template>
  <div class="home">
    <Carousel />
    <MainContainer>  
    </MainContainer>
  </div>
</template>

<script>
import MainContainer from '@/components/MainContainer.vue'
import Carousel from '@/components/Carousel.vue';

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Home',
  components: {
    MainContainer,
    Carousel
  }
}
</script>
