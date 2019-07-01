<template>
  <div :class="{ 'blue': isBlue }"></div>
</template>

<script>
export default {
  name: 'v-bind',

  computed: {
    isBlue () {
      return Math.random(0, 1) > 0.5
    }
  }
}
</script>

<style>
div {
  background: red;
}

div.blue {
  background: blue;
}
</style>
