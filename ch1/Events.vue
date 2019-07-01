<template>
  <div>
    <!--<button @click="clickHandler">Click me!</button>-->
    <button @click.prevent.stop="clickHandler">Click me!</button>
  </div>
</template>

<script>
export default {
  name: 'events',

  methods: {
    clickHandler (event) {
      /*event.preventDefault()
      event.stopPropagation()*/
    }
  }
}
</script>
