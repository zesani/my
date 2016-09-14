<template>

  <div class="box">

 <img :src="img" width="450px"> <br>
 <button @click="previous" disabled="{{page==1}}"> previous </button>
 <button > {{page}} </button>
 <button @click="next" disabled="{{page==26}}"> next </button>

 </div>


</template>

<script>
export default {
  data () {
    return {
      page: 1
    }
  },
  computed: {
    img: function () {
      return 'http://bill.sellsuki.com/cartoon/' + this.page + '.jpg'
    }
  },
  methods: {
    previous: function () {
      this.page--
    },
    next: function () {
      this.page++
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
