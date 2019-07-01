<template>
  <button :click="save">Save</button>
</template>

<script>
export default {
  name: 'person',

  data () {
    return {
      name: 'Stu Ratcliffe'
    }
  },

  methods: {
    save () {
      this.$emit('name-changed', this.name)
    }
  }
}
</script>
