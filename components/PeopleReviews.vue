<template>
  <div class="container">
    <div class="row text-center text-lg-start">
      <div class="col col-12 col-md-6">
        <h1 class="text-white">
          What people are saying about us
        </h1>
      </div>
      <div class="col col-12 col-md-6 d-flex flex-column align-items-center justify-content-center">
        <p class="text-primary m-0 mt-3 mb-2">
          Everything you need to accept card payments and grow your business anywhere on the planet.
        </p>
      </div>
    </div>
    <div class="row py-3">
      <div v-for="cardDetails in reviewCards" class="col col-12 col-md-6 col-lg-4 mt-4">
        <review-card :card-details="cardDetails"/>
      </div>
    </div>
  </div>
</template>

<script>
import ReviewCard from "@/components/ReviewCard";

export default {
  name: "PeopleReviews",
  components: {ReviewCard},
  data() {
    return {
      reviewCards: [
        {
          img: require('../assets/images/people-reviews/herman.svg'),
          alt: 'Herman Jensen image',
          name: 'Herman Jensen',
          description: 'Founder & Leader',
          text: 'Money is only a tool. It will take you wherever you wish, but it will not replace you as the driver.',
        },
        {
          img: require('../assets/images/people-reviews/steve.svg'),
          alt: 'Steve Mark image',
          name: 'Steve Mark',
          description: 'Founder & Leader',
          text: 'Money makes your life easier. If you\'re lucky to have it, you\'re lucky.',
        },
        {
          img: require('../assets/images/people-reviews/kenn.svg'),
          alt: 'Kenn Gallagher image',
          name: 'Kenn Gallagher',
          description: 'Founder & Leader',
          text: 'It is usually people in the money business, finance, and international trade that are really rich.',
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

p {
  font-size: 18px;
  font-weight: 400;
}
</style>
