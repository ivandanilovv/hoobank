<template>
  <div class="custom-bg-color">
    <custom-navbar/>
    <hero-section/>
    <div class="position-relative">
      <div class="position-absolute w-65 h-75 top-0 start-minus-60 left-gradient"/>
      <features/>
      <billing-and-invoicing/>
    </div>
    <card-deal/>
  </div>
</template>

<script>
import CustomNavbar from "~/components/CustomNavbar";
import HeroSection from "@/components/HeroSection";
import Features from "@/components/Features";
import BillingAndInvoicing from "@/components/BillingAndInvoicing";
import CardDeal from "@/components/CardDeal";

export default {
  name: 'IndexPage',
  components: {
    CardDeal,
    BillingAndInvoicing,
    Features,
    HeroSection,
    CustomNavbar
  },
  head: {
    title: 'HooBank',
  }
}
</script>
