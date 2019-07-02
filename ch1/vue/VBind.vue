<template>
  <img v-bind:src="imageSrc" alt="image" />
</template>

<script>
export default {
  name: 'v-bind',

  data () {
    return {
      imageSrc: '',
      images: [
        'path/to/image/1.jpg',
        'path/to/image/2.jpg',
        'path/to/image/3.jpg'
      ]
    }
  },

  mounted () {
    let count = 0

    setInterval(() => {
      this.imageSrc = this.images[count++]

      if (count === this.images.length) {
        count = 0
      }
    }.bind(this), 1.5 * 1000)
  }
}
</script>
