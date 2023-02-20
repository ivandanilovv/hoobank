<template>
  <div class="container">
    <div class="row">
      <div class="col col-12 col-md-6 mt-5 pt-8 position-relative">
        <div class="discount-bg-color p-2 rounded-3 w-65 fs-7 d-flex flex-row align-items-center">
          <img src="../assets/images/hero-section/discount-icon.svg" alt="Discount icon" class="ms-1"/>
          <span class="text-white ms-2">
            20% <span class="text-primary">DISCOUNT FOR</span> 1 MONTH <span class="text-primary">ACCOUNT</span>
          </span>
        </div>
        <h1 class="text-white pt-3 pb-5">
          The Next<br/><span class="custom-font-gradient">Generation</span><br/> Payment Method.
        </h1>
        <p class="text-primary m-0">
          Our team of experts uses a methodology to identify<br/> the credit cards most likely to fit your needs.<br/>
          We examine annual percentage rates, annual fees.
        </p>
        <div class="position-absolute w-65 h-75 top-0 start-minus-60 left-gradient"/>
      </div>
      <div
        class="col col-12 col-md-6 p-0 py-5 d-flex flex-row justify-content-end align-items-center position-relative">
        <div class="ratio ratio-1x1">
          <img src="../assets/images/hero-section/hand.svg" alt="Hand"/>
        </div>
        <div class="position-absolute w-80 h-60 top-0 end-10 right-gradient"/>
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

.w-80 {
  width: 80% !important;
}

.h-60 {
  height: 60% !important;
}

.end-10 {
  right: 10%;
}

.start-minus-60 {
  left: -60%;
}

.w-65 {
  width: 65% !important;
}

.h-75 {
  height: 75% !important;
}

.right-gradient {
  background: linear-gradient(180deg, rgba(188, 165, 255, 0) 0%, #214D76 100%);
  border: 1px solid #000000;
  filter: blur(61.5px);
}

.left-gradient {
  background: linear-gradient(180deg, rgba(188, 165, 255, 0) 0%, #214D76 100%);
  border: 1px solid #000000;
  filter: blur(130.5px);
}

.fs-7 {
  font-size: 18px;
}

.discount-bg-color {
  background-color: #1b1b22;
}
</style>
