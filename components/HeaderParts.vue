<template>
    <header class="pt-8 pl-4 md:px-12 flex justify-between relative">
        <img src="~assets/images/logo.png">
        <ul class="hidden md:flex justify-between text">
          <li>
            <nuxt-link to="/" class="relative inline-block mx-4 link-color active">Learn</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/home" class="relative inline-block mx-4 link-color">Categories</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/home" class="relative inline-block mx-4 link-color">Stories</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/home" class="relative inline-block mx-4 link-color">Partner</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/home" class="relative inline-block mx-4 link-color">Investor</nuxt-link>
          </li>
        </ul>
      </header>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

</style>