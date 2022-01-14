<template>
  <div>
    <h2> {{title }}</h2>
    <h4> {{ author}} </h4>
  </div>
</template>

<script>
export default {
  name: 'bookInfo',
  props: {
    title: String, 
    author: String,
  },
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
a {
  color: #42b983;
}
</style>