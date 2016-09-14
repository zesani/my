<template>
  <div class="hello">
    <!-- <h1>{{ msg }}</h1> -->
    <display2 :msg="msg"></display2>
  </div>
</template>

<script>
import Display2 from './Display2'

export default {
  props: ['msg'],
  data () {
    return {
    }
  },
  components: {
    Display2
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}
</style>
