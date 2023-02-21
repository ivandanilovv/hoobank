<template>
  <div class="custom-bg-color">
    <custom-navbar/>
    <hero-section/>
    <features/>
    <billing-and-invoicing/>
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
