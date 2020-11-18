<template>
  <div class="competence">
    <h3>{{ title }}</h3>
    <ul>
      <li v-for="competence in competencies" :key="competence">{{ competence }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Competence',
  props: {
    title: String,
    competencies: Array
  }
}
</script>

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
