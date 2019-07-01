<template>
  <div>
    {{ fullName }}
  </div>
</template>

<script>
export default {
  name: 'computed-properties',

  data () {
    return {
      firstName: 'Stu',
      lastName: 'Ratcliffe'
    }
  },

  computed: {
    fullName () {
      const { firstName, lastName } = this

      return `${firstName} ${lastName}`
    }
  }
}
</script>
