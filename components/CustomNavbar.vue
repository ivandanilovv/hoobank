<template>
  <div>
    <nav class="navbar navbar-expand-md">
      <div class="container">
        <a class="navbar-brand" href="#">
          <img src="../assets/images/custom-navbar/logo.png" alt="Logo image" width="92"/>
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
                aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon bg-primary p-3 rounded-3"></span>
        </button>
        <div class="collapse navbar-collapse d-md-flex flex-row align-items-end justify-content-end" id="navbarNav">
          <ul class="navbar-nav align-items-center">
            <li class="nav-item" v-for="(item, i) in navbarItems" :class="{'me-md-5' : i !== navbarItems.length - 1}">
              <a class="nav-link text-primary" aria-current="page" :href="item.link" :class="{'active' : i === 0}">
                {{ item.text }}
              </a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "CustomNavbar",
  data() {
    return {
      navbarItems: [
        {
          text: 'Home',
          link: '#',
        },
        {
          text: 'About Us',
          link: '#',
        },
        {
          text: 'Features',
          link: '#',
        },
        {
          text: 'Solution',
          link: '#',
        },
      ]
    }
  }
}
</script>

<style scoped>
.active {
  color: white !important;
  font-weight: bold;
}

a:hover {
  color: grey !important;
}
</style>
