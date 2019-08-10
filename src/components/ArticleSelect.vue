<template lang="html">
<select @change="" >
  <option selected disabled></option>
  <option value=""></option>

</select>
</template>

<script>
export default {
  name: 'article-select',
  props: ['articles']
}
</script>

<style lang="css" scoped>
</style>
