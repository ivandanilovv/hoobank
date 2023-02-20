<template>
  <div class="custom-bg-color">
    <custom-navbar/>
    <hero-section/>
  </div>
</template>

<script>
import CustomNavbar from "~/components/CustomNavbar";
import HeroSection from "@/components/HeroSection";
export default {
  name: 'IndexPage',
  components: {HeroSection, CustomNavbar},
  head: {
    title: 'HooBank',
  }
}
</script>
