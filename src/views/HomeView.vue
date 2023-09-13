<template>
  <div class="home">
    <Carousel />
    <div class="container home__offering">
      <div class="row">
        <div class="col-md-4 home__border">
          <h3 class="home__offeringTitle">
            We are offering the best Estate Details
          </h3>
        </div>
        <div class="col-md-8">
          <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Minus numquam, blanditiis repellat autem cumque, quaerat voluptate temporibus, voluptas consectetur vel nisi. Voluptatem, sint pariatur perspiciatis libero consectetur vitae neque ea?
          </p>
        </div>
      </div>
    </div>
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
