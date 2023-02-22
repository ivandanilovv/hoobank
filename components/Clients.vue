<template>
  <div class="container py-3">
    <div class="row">
      <div class="col col-12 col-sm-6 col-lg-3 d-flex flex-row align-items-center justify-content-center mt-sm-2"
           v-for="(image, i) in clientsImages" :class="{'mt-4' : i !== 0}">
        <a :href="image.link" target="_blank">
          <img :src="image.src" :alt="image.alt"/>
        </a>
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
          alt: 'Airbnb Logo',
          link: 'https://www.airbnb.com/',
        },
        {
          src: require('../assets/images/clients/binance.svg'),
          alt: 'Binance Logo',
          link: 'https://www.binance.com/en'
        },
        {
          src: require('../assets/images/clients/coinbase.svg'),
          alt: 'Coinbase Logo',
          link: 'https://www.coinbase.com/'
        },
        {
          src: require('../assets/images/clients/dropbox.svg'),
          alt: 'Dropbox Logo',
          link: 'https://www.dropbox.com/'
        },
      ]
    }
  }
}
</script>

<style scoped>

</style>
