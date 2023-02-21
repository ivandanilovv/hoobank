<template>
  <div class="container py-3 py-md-5 mt-lg-5">
    <div class="row">
      <div class="col col-12 col-md-6 text-center text-md-start">
        <h1 class="text-white m-0">
          You do the business,<br class="d-none d-lg-block"/>
          we’ll handle the money.
        </h1>
        <p class="text-primary m-0 py-4 fs-6">
          With the right credit card, you can improve your financial life by<br class="d-none d-lg-block"/>
          building credit, earning rewards and saving money. But with<br class="d-none d-lg-block"/>
          hundreds of credit cards on the market.
        </p>
        <a href="#" class="btn custom-button-style rounded-3 py-3 px-5 mt-2">
          Get Started
        </a>
      </div>
      <div class="col col-12 col-md-6 col-xl-5 offset-xl-1 pt-4 pt-md-0">
        <div class="d-flex flex-row mb-3 rounded-4 p-3 hover-gradient" v-for="item in featureItems">
          <img :src="item.image" :alt="item.alt" width="64" height="64"/>
          <div class="d-flex flex-column ms-3">
            <h5 class="text-white">
              {{ item.header }}
            </h5>
            <p class="text-primary m-0">
              {{ item.text }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Features",
  data() {
    return {
      featureItems: [
        {
          image: require('../assets/images/features/image1.svg'),
          alt: 'Image 1',
          header: 'Rewards',
          text: 'The best credit cards offer some tantalizing combinations of promotions and prizes'
        },
        {
          image: require('../assets/images/features/image2.svg'),
          alt: 'Image 2',
          header: '100% Secured',
          text: 'We take proactive steps make sure your information and transactions are secure.'
        },
        {
          image: require('../assets/images/features/image3.svg'),
          alt: 'Image 3',
          header: 'Balance Transfer',
          text: 'A balance transfer credit card can save you a lot of money in interest charges.'
        },
      ]
    }
  }
}
</script>

<style scoped>
h1 {
  font-size: 48px;
  font-weight: 600;
}

h5 {
  font-size: 18px;
  font-weight: 600;
}

.fs-6 {
  font-size: 18px;
}

.hover-gradient:hover {

  /* ff 3.6+ */
  background:-moz-linear-gradient(180deg, rgba(46, 44, 55, 1) 0%, rgba(26, 21, 34, 1) 100%);

  /* safari 5.1+,chrome 10+ */
  background:-webkit-linear-gradient(180deg, rgba(46, 44, 55, 1) 0%, rgba(26, 21, 34, 1) 100%);

  /* opera 11.10+ */
  background:-o-linear-gradient(180deg, rgba(46, 44, 55, 1) 0%, rgba(26, 21, 34, 1) 100%);

  /* ie 6-9 */
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#1A1522', endColorstr='#2E2C37', GradientType=1 );

  /* ie 10+ */
  background:-ms-linear-gradient(180deg, rgba(46, 44, 55, 1) 0%, rgba(26, 21, 34, 1) 100%);

  /* global 94%+ browsers support */
  background:linear-gradient(180deg, rgba(46, 44, 55, 1) 0%, rgba(26, 21, 34, 1) 100%);
}

</style>
