<template>
  <h3><span>{{ title }}</span> {{ text }}</h3>
</template>

<script>
export default {
  name: "list-home",
  props:[
      'title',
      'text'
  ]
}
</script>

<style scoped>

</style>