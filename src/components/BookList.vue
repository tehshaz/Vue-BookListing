<template>
  <div>
    <h1>{{ title }}</h1>
    <ul>
      <li li v-for="book in books" :key="book.id">{{ book.title }}:{{ book.author }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "BookList",
      title: "All Books",
      books: [
        { title: "Self-Reliance", author: "Ralph Waldo Emerson" },
        { title: "American Gods", author: "Neil Gaiman" },
        { title: "Amusing Ourselves to Death", author: "Neil Postman" }
      ]
    };
  }
};
</script>

<style>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
</style>