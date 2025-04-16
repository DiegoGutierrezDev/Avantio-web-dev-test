<script setup>
const props = defineProps(['text'])
</script>

<template>
<button class="AppButton">
  {{ text }}
</button>
</template>

<style lang="scss" scoped>
.AppButton {
  padding: 0.5rem;
  border-radius: 1rem;
  font-size: 1rem;
  color: white;
  background-color: $avantio-orange;
}
</style>