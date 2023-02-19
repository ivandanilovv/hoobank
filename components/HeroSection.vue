<template>
  <div class="container">
    <div class="row">
      <div class="col col-6 mt-5 pt-8">
        <span style="background-color: #1b1b22;" class="p-2 rounded-3 pb-3">
          <img src="../assets/images/hero-section/discount.svg" alt="Discount"/>
        </span>
        <h1 class="text-white pt-3 pb-5">
          The Next<br/><span class="custom-font-gradient">Generation</span><br/> Payment Method.
        </h1>
        <p class="text-primary m-0">
          Our team of experts uses a methodology to identify<br/> the credit cards most likely to fit your needs.<br/>
          We examine annual percentage rates, annual fees.
        </p>
      </div>
      <div class="col col-6 p-0 py-5 d-flex flex-row justify-content-end">
        <div class="ratio ratio-1x1">
          <img src="../assets/images/hero-section/hand.svg" alt="Hand" class=""/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeroSection"
}
</script>

<style scoped>
h1 {
  font-size: 72px;
  font-weight: 600;
}

p {
  font-size: 18px;
  font-weight: 400;
}

.pt-8 {
  padding-top: 8rem !important;
}
</style>
