<template>
  <form v-on:submit.prevent="bookSubmit(bookTitle, bookAuthor)" class="" action="#" method="post">
    <input v-model="bookTitle" type="text" name="title" value="" place-holder="Book Title">
    <input v-model="bookAuthor" type="text" name="author" value="" place-holder="Book Author">
    <input type="submit" name="button">Add Book</button>
  </form>
</template>

<script>
export default {
  name: "BookForm",
  props: ['books'],
  data: function() {
    return {
      bookTitle: '',
      bookAuthor: ''
    }
  },
  methods: {
    bookSubmit: function(bookTitle, bookAuthor)
    {
      this.$emit('addBook', bookTitle, bookAuthor);
    }
  }
}
</script>

<style>
</style>
