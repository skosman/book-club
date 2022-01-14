<template>
  <div >
    <li v-for="book in books" :key="book.id">
      <book-info
        :title="book.title"
        :author="book.author"
      />
    </li>
  </div>
</template>

<script>
import BookInfo from './BookInfo.vue'
export default {
  name: 'HelloWorld',
  components: {
    BookInfo,
  },
  data() {
    return {
      books: [
        {
          title: "Book",
          author: "Test Tester",
        },
        {
          title: "Book Name",
          author: "Author Author",
        },
      ]
    }
  }  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
