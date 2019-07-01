<template>
  <input v-bind:value="message" />
</template>

<script>
export default {
  name: 'data-binding',

  data () {
    return {
      message: 'Hands on Vue.js and ASP.NET Core'
    }
  }
}
</script>
