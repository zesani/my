<template>
    <button @click="onClick()">Edit</button>
    <!-- <button >Edit2</button> -->
</template>

<script>
export default {
  props: ['onClick'],
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
