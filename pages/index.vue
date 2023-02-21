<template>
  <div class="custom-bg-color">
    <custom-navbar/>
    <hero-section/>
    <features/>
  </div>
</template>

<script>
import CustomNavbar from "~/components/CustomNavbar";
import HeroSection from "@/components/HeroSection";
import Features from "@/components/Features";
export default {
  name: 'IndexPage',
  components: {Features, HeroSection, CustomNavbar},
  head: {
    title: 'HooBank',
  }
}
</script>
