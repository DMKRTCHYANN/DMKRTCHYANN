<template>
  <div class="flex flex-col items-center justify-center h-screen bg-gray-100">
    <home-button @vren-pahec="asdf" title="Login" link="/login"></home-button>
    <home-button title="Register" link="/register"></home-button>
  </div>
</template>

<script setup lang="ts">

import HomeButton from "~/components/HomeButton.vue";


const asdf = (a, b) => {
  console.log(a, b)
}


</script>

<style scoped>

</style>



