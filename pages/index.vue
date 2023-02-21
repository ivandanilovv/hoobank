<template>
  <div class="custom-bg-color">
    <custom-navbar/>
    <hero-section/>
    <div class="position-relative">
      <div class="position-absolute w-65 h-75 top-0 start-minus-60 left-gradient"/>
      <features/>
      <billing-and-invoicing/>
    </div>
  </div>
</template>

<script>
import CustomNavbar from "~/components/CustomNavbar";
import HeroSection from "@/components/HeroSection";
import Features from "@/components/Features";
import BillingAndInvoicing from "@/components/BillingAndInvoicing";

export default {
  name: 'IndexPage',
  components: {
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
