<template>
  <!--<input type="text" :value="value" @input="onInputChange" />-->
  <input type="text" v-model="value" />
</template>

<script>
export default {
  name: 'form-input-binding',

  data () {
    return {
      value: 'Some value'
    }
  },

  methods: {
    /*onInputChange (event) {
      this.value = event.target.value
    }*/
  }
}
</script>
