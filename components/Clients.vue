<template>
  <div class="container py-3">
    <div class="row">
      <div class="col col-12 col-sm-6 col-lg-3 d-flex flex-row align-items-center justify-content-center mt-sm-2"
           v-for="(image, i) in clientsImages" :class="{'mt-4' : i !== 0}">
          <img :src="image.src" :alt="image.alt"/>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Clients",
  data() {
    return {
      clientsImages: [
        {
          src: require('../assets/images/clients/airbnb.svg'),
          alt: 'Airbnb Logo'
        },
        {
          src: require('../assets/images/clients/binance.svg'),
          alt: 'Binance Logo'
        },
        {
          src: require('../assets/images/clients/coinbase.svg'),
          alt: 'Coinbase Logo'
        },
        {
          src: require('../assets/images/clients/dropbox.svg'),
          alt: 'Dropbox Logo'
        },
      ]
    }
  }
}
</script>

<style scoped>

</style>
