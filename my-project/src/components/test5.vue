<template>

  <div class="leftBox">
R : <input v-model="R"><br><br>
G : <input v-model="G"><br><br>
B : <input v-model="B"><br><br>

</div>
<div class="box" style="{{color}}"></div>
<button @click="randomColor">random</button>
</template>

<script>
export default {
  data () {
    return {
      R: 255,
      G: 0,
      B: 0
    }
  },
  computed: {
    color: function () {
      return 'background-color: rgb(' + this.R + ', ' + this.G + ', ' + this.B + ')'
    }
  },
  methods: {
    randomColor: function () {
      this.R = Math.floor((Math.random() * 255))
      this.G = Math.floor((Math.random() * 255))
      this.B = Math.floor((Math.random() * 255))
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.box{
  width: 300px;
  height:300px;
}
</style>
