<template>
  <input class="input" type="text" :placeholder="placeholder" />
</template>

<script>
export default {
  name: "Input",
  props: ["placeholder"],
};
</script>

<style scoped src="./Input.css">
</style>

