<template>
  <div>
    <h1>Watchers Example</h1>
    <input v-model="searchValue" />
    <span v-show="loading">Loading...</span>
    <ul>
      <li v-for="result in searchResults">{{ result }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'watchers',

  data () {
    return {
      loading: false,
      searchResults: [],
      searchValue: '',
    }
  },

  watch: {
    searchValue (newValue) {
      this.loading = true

      setTimeout(() => {
        this.searchResults.push('some', 'search', 'results')
        this.loading = false
      }, 0.5 * 1000).bind(this)
    }
  }
}
</script>
