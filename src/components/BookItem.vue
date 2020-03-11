<template>
  <div>
    <ol>
      <li>{{ book.title }}:{{ book.author }}</li>
    </ol>
  </div>
</template>

<script>
  export default {
    name: 'BookItem',
    props: [
      'book',
    ],
  }
</script>

<style>
li {
  display: block;
  margin: 0 10px;
}
</style>