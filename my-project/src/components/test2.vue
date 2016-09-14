<template>

    <div class="box">
      {{number}}
      <button @click="plus"> + </button>
      <button @click="minus" :disabled="check"> - </button>
    </div>


</template>

<script>
export default {
  data () {
    return {
      number: 0,
      check: true
    }
  },
  methods: {
    plus: function () {
      this.number++
      this.check = false
    },
    minus: function () {
      this.number--
      if (this.number === 0) {
        this.check = true
      }
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
