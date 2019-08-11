<template lang="html">

  <ul v-if="article !== null">
    <h3>{{article.webTitle}}</h3>
    <p>Section: {{article.sectionName}}</p>
    <p>Link to the article:</p>
    <a v-bind:href="article.webUrl">link</a>
  </ul>

</template>

<script>
export default {
  name: 'display-article',
  props: ['article']
}
</script>

<style lang="css" scoped>
</style>
