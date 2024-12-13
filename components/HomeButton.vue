<template>
  <div @mouseover="onHover">
    <NuxtLink :to="link" >
      <button
          class="w-[300px] rounded-[10px] bg-[#3A5B22] font-bold text-white px-2 py-2  cursor-pointer flex justify-center items-center mb-4">
        {{ title }}
      </button>
    </NuxtLink>
  </div>
</template>

<script setup lang="ts">
defineProps({
  title: {
    type: String,
    required: true,
  },
  link: {
    type: String,
    required: true,
  }
})

const emit = defineEmits(["vrenPahec"])

const onHover = () => {
  emit("vrenPahec", "asdasdsa", "dasdasdsadasdas");
}


</script>

<style scoped>

</style>