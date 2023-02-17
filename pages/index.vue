<template>
  <div class="custom-bg-color">
    <custom-navbar/>
  </div>
</template>

<script>
import CustomNavbar from "~/components/CustomNavbar";
export default {
  name: 'IndexPage',
  components: {CustomNavbar},
  head: {
    title: 'HooBank',
  }
}
</script>
