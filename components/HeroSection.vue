<template>
  <div class="container">
    <div class="row">
      <div class="col col-12 col-lg-6 mt-5 pt-8 position-relative text-center text-lg-start
                  d-flex flex-column justify-content-center align-items-center align-items-lg-start">
        <div class="discount-bg-color p-2 rounded-3 discount-width fs-7
          d-flex flex-row align-items-center justify-content-center justify-content-lg-start">
          <img src="../assets/images/hero-section/discount-icon.svg" alt="Discount icon" class="ms-1"/>
          <span class="text-white ms-2">
            20% <span class="text-primary">DISCOUNT FOR</span> 1 MONTH <span class="text-primary">ACCOUNT</span>
          </span>
        </div>
        <h1 class="text-white pt-3 pb-5">
          The Next<br/><span class="custom-font-gradient">Generation</span><br/> Payment Method.
        </h1>
        <p class="text-primary m-0">
          Our team of experts uses a methodology to identify<br class="d-none d-md-block"/>
          the credit cards most likely to fit your needs.<br class="d-none d-md-block"/>
          We examine annual percentage rates, annual fees.
        </p>
        <div class="position-absolute w-65 h-75 top-0 start-minus-60 left-gradient"/>
      </div>
      <div
        class="col col-12 col-lg-6 p-0 py-5 d-flex flex-row justify-content-end align-items-center position-relative">
        <div class="ratio ratio-1x1">
          <img src="../assets/images/hero-section/hand.svg" alt="Hand"/>
        </div>
        <div class="position-absolute w-80 h-60 top-0 end-10 right-gradient"/>
      </div>
    </div>
    <div class="row py-5 px-3">
      <div v-for="(item, i) in usersItems"
           class="col col-12 col-lg-4 d-flex flex-row align-items-center p-0"
           :class="item.class">
        <span class="custom-border-left d-none" :class="{'d-lg-block' : i === 1}"/>
        <h2 class="text-white">
          {{ item.number }}
        </h2>
        <div class="custom-font-gradient fs-5 fw-normal ms-3">
          {{ item.text }}
        </div>
        <span class="custom-border-right d-none" :class="{'d-lg-block' : i === 1}"/>
      </div>
    </div>
<!--    <div class="py-5 px-3 d-flex flex-row align-items-center justify-content-evenly">-->
<!--      <div class="d-flex flex-row align-items-center">-->
<!--        <h2 class="text-white">-->
<!--          3800+-->
<!--        </h2>-->
<!--        <div class="custom-font-gradient fs-5 fw-normal ms-3">-->
<!--          USER ACTIVE-->
<!--        </div>-->
<!--      </div>-->
<!--      <div class="d-flex flex-row align-items-center">-->
<!--        <span class="custom-border-left"/>-->
<!--        <h2 class="text-white">-->
<!--          230+-->
<!--        </h2>-->
<!--        <div class="custom-font-gradient fs-5 fw-normal ms-3">-->
<!--          TRUSTED BY COMPANY-->
<!--        </div>-->
<!--      </div>-->
<!--      <span class="custom-border-right"/>-->
<!--      <div class="d-flex flex-row align-items-center">-->
<!--        <h2 class="text-white">-->
<!--          $230M+-->
<!--        </h2>-->
<!--        <div class="custom-font-gradient fs-5 fw-normal ms-3">-->
<!--          TRANSACTION-->
<!--        </div>-->
<!--      </div>-->
<!--    </div>-->
  </div>
</template>

<script>
export default {
  name: "HeroSection",
  data() {
    return {
      usersItems: [
        {
          number: '3800+',
          text: 'USER ACTIVE',
          class: 'justify-content-center justify-content-sm-start'
        },
        {
          number: '230+',
          text: 'TRUSTED BY COMPANY',
          class: 'justify-content-center justify-content-lg-between'
        },
        {
          number: '$230M+',
          text: 'TRANSACTION',
          class: 'justify-content-center justify-content-sm-end'
        }
      ]
    }
  }
}
</script>

<style scoped>
.w-65 {
  width: 65% !important;
}

@media (min-width: 1200px){
  .discount-width {
    width: 65% !important;
  }
}

@media (min-width: 992px) {
  .pt-8 {
    padding-top: 8rem !important;
  }
}

.custom-border-right {
  border-left: rgba(255, 255, 255, 0.6) 1.70386px solid;
  height: 30% !important;
}

.custom-border-left {
  border-left: rgba(255, 255, 255, 0.6) 1.70386px solid;
  height: 30% !important;
}

h1 {
  font-size: 72px;
  font-weight: 600;
}

h2 {
  font-size: 40px;
  font-weight: 600;
}

p {
  font-size: 18px;
  font-weight: 400;
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
