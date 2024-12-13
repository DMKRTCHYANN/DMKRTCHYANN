<template>
<div>
  <input :value="modelValue" @input="asdf($event)" class="w-full p-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-[#3A5B22]"/>
</div>
</template>


<script setup>

defineProps(['modelValue'])
const emit = defineEmits(["update:modelValue"])

const asdf = (e) => {
  emit("update:modelValue", e.target.value);
}
</script>


