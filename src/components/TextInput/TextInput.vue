<template>
  <textarea class="text-area" name="" id="" cols="30" rows="10" :placeholder="placeholder"></textarea>
</template>

<script>
export default {
  name: "TextInput",
  props: ["placeholder"],
};
</script>

<style scoped src="./TextInput.css">
</style>

