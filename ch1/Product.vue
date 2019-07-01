<template>
  <div class="product">
    <child-component name="Hands on Vue.js and ASP.NET Core" />
  </div>
</template>

<script>
import ChildComponent from './ChildComponent.vue'

export default {
  name: 'parent',

  components: {
    ChildComponent
  }
}
</script>
