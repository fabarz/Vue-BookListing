<template>
  <h1>{{ title }}</h1>
</template>

<script>
export default {
  name: "Book list",
  data: function() {
    return {
      title: "All Books"
    }
  }
}
</script>

<style>
  h1, h2 {
    font-weight: normal
  }
</style>
