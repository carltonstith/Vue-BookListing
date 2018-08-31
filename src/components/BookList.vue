<template lang="html">
  <div class="book-list">
    <h1>{{title}}</h1>
    <ul>
      <book-item v-for="book in books" :book="book"></book-item>
    </ul>
  </div>
</template>

<script>
import BookItem from './BookItem';

export default {
  name: 'BookList',
  data () {
    return  {
        title: 'All Books',
        books: [
          {title: 'Self-Reliance', author: 'Ralph Waldo Emmerson'},
          {title: 'American Gods', author: 'Neil Gaiman'},
          {title: 'Amusing Ourselves to Death', author: 'Neil Postman'}
        ]
    }
  },
  components: {
    BookItem
  }
}
</script>

<style lang="css">
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
</style>
