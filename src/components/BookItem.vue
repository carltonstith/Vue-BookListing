<template lang="html">
  <li>{{book.title}}: {{book.author}}</li>
</template>

<script>
export default {
  name: 'BookItem',
  props: ['book']
}
</script>

<style lang="css">
li {
  display: block;
  margin: 0 10px;
}
</style>
