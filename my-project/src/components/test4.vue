<template>

  <center>
     <img :src="foodPhotos[number]"><br>
     {{number}}
     <button v-on:click="random()" >Random</button>
   </center>


</template>

<script>
export default {
  data () {
    return {
      number: 1,
      foodPhotos: ['https://pixabay.com/static/uploads/photo/2016/07/23/07/08/tofu-1536355__180.jpg',
     'https://pixabay.com/static/uploads/photo/2016/08/03/04/42/shrimp-1565873__180.jpg',
     'https://pixabay.com/static/uploads/photo/2015/08/26/10/58/vermicelli-salad-908334__180.jpg',
     'https://pixabay.com/static/uploads/photo/2016/03/05/22/09/appetite-1239198__180.jpg',
     'https://pixabay.com/static/uploads/photo/2016/03/05/19/55/barbeque-1238552__180.jpg',
     'https://pixabay.com/static/uploads/photo/2016/03/05/21/46/american-1239080__180.jpg',
     'https://pixabay.com/static/uploads/photo/2016/07/28/19/53/food-1549252__180.jpg',
     'https://pixabay.com/static/uploads/photo/2015/09/04/11/00/colorful-921902__180.jpg',
     'https://pixabay.com/static/uploads/photo/2014/11/25/14/55/noodles-545259__180.jpg',
     'https://pixabay.com/static/uploads/photo/2015/04/03/17/49/rotisserie-chicken-705575__180.jpg',
     'https://pixabay.com/static/uploads/photo/2016/08/09/15/09/noodle-1580833__180.jpg',
     'https://pixabay.com/static/uploads/photo/2016/07/28/17/01/fish-ball-1548468__180.jpg',
     'https://pixabay.com/static/uploads/photo/2016/08/03/04/45/pork-1565882__180.jpg',
     'https://pixabay.com/static/uploads/photo/2016/07/23/07/54/pork-1536414__180.jpg',
     'https://pixabay.com/static/uploads/photo/2016/08/09/15/19/fried-1580879__180.jpg',
     'https://pixabay.com/static/uploads/photo/2015/07/08/07/06/sausage-835433__180.jpg',
     'https://pixabay.com/static/uploads/photo/2015/12/13/03/32/food-1090619__180.jpg',
     'https://pixabay.com/static/uploads/photo/2015/05/23/22/04/omelette-781105__180.jpg',
     'https://pixabay.com/static/uploads/photo/2016/04/24/05/36/fish-ball-1348826__180.jpg',
     'https://pixabay.com/static/uploads/photo/2016/07/28/19/58/rice-1549343__180.jpg',
     'https://pixabay.com/static/uploads/photo/2016/07/28/19/54/dessert-1549271__180.jpg']
    }
  },
  methods: {
    random: function () {
      this.number = Math.floor(Math.random() * (21) + 0)
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
