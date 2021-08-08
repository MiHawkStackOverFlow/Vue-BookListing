<template>
  <div>
    <li v-for="book in books" :key="book.title">
      {{ book.title }} : {{ book.author }}
    </li>
  </div>
</template>

<script>
export default {
  name: "BookItem",
  props: ["books"]
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
li {
  display: block;
  margin: 0 10px;
}
</style>
