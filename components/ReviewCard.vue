<template>
  <div class="p-5 rounded-4 h-100 d-flex flex-column justify-content-between card-background-gradient">
    <img src="../assets/images/people-reviews/quotation-mark.svg" alt="Quotation mark" width="43" height="28"/>
    <p class="text-primary py-4">
      {{ cardDetails.text }}
    </p>
    <div class="row">
      <div class="col col-3 d-flex flex-column justify-content-center">
        <div class="ratio ratio-1x1">
        <img :src="cardDetails.img" :alt="cardDetails.alt"/>
        </div>
      </div>
      <div class="col col-9 d-flex flex-column justify-content-center">
        <h5 class="text-white m-0">
          {{ cardDetails.name }}
        </h5>
        <p class="text-primary m-0">
          {{cardDetails.description}}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ReviewCard",
  props: {
    cardDetails: Object,
  }
}
</script>

<style scoped>
h5 {
  font-size: 20px;
  font-weight: 400;
}

p {
  font-size: 18px;
  font-weight: 400;
}

.card-background-gradient {

  /* ff 3.6+ */
  background:-moz-linear-gradient(180deg, rgba(79, 77, 86, 1) 0%, rgba(20, 16, 29, 1) 100%);

  /* safari 5.1+,chrome 10+ */
  background:-webkit-linear-gradient(180deg, rgba(79, 77, 86, 1) 0%, rgba(20, 16, 29, 1) 100%);

  /* opera 11.10+ */
  background:-o-linear-gradient(180deg, rgba(79, 77, 86, 1) 0%, rgba(20, 16, 29, 1) 100%);

  /* ie 6-9 */
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#14101D', endColorstr='#4F4D56', GradientType=1 );

  /* ie 10+ */
  background:-ms-linear-gradient(180deg, rgba(79, 77, 86, 1) 0%, rgba(20, 16, 29, 1) 100%);

  /* global 94%+ browsers support */
  background:linear-gradient(180deg, rgba(79, 77, 86, 1) 0%, rgba(20, 16, 29, 1) 100%);
}
</style>
