<template>
  <div class="hello">
    {{index+1}}.
  {{list.name}}
    <button @click="remove(index)">X</button>
  </div>
</template>

<script>
export default {
  props: ['list', 'remove', 'index'],
  data () {
    return {

    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}
</style>
