<template>
  <div class="properties">
    <div class="container">
      <div class="row">
        <div class="col">
          <h2 class="properties__h2">Featured
            <b>Properties</b>
          </h2>
        </div>
        <div class="col">
          <div class="properties__subtitle">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dicta, cupiditate.
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-md-4 col-sm-12" v-for="property in propertiesData" :key="property.id">
          <div class="properties__col">
            <img class="properties__img" :src="require(`../assets/images/${property.image}.png`)" :alt="property.desc.sqft"/>
            <h4 class="properties__h4">{{ `${property.desc.sqft} ${property.title}` }}</h4>
            <p class="properties__sub">{{ property.subtitle }}</p>
            <p class="properties__price">{{ property.price }}</p>
            <ul class="properties__desc">
              <li class="properties__item">{{ property.desc.sqft }} sq ft</li>
              <li class="properties__item">{{ property.rooms }} Bedrooms</li>
              <li class="properties__item">{{ property.bath }} Bathrooms</li>
            </ul>
          </div>
          <div class="col">
            <button type="button" class="btn btn-primary properties__item properties__more">All Properties</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  props: {
    propertiesData: {
      type: Array,
      default: () => [],
    }
  }
}
</script>