<template>
  <div id="app">

  </div>
</template>

<script>


export default {
  data(){
    return {
      articles: [],
    }
  },
  mounted(){
    fetch('https://content.guardianapis.com/search?q=brexit&format=json&api-key=test')
    .then(res => res.json())
    .then(banana => this.articles = banana)
    




  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
