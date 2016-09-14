<template>
  <div id="app">
    <test1></test1>
    <hr>
    <test3></test3>
    <hr>
    <test4></test4>
    <hr>
    <test5></test5>
    <hr>
  </div>
</template>

<script>
import Hello from './components/Hello'
import test1 from './components/test1'
import test3 from './components/test3'
import test4 from './components/test4'
import test5 from './components/test5'
export default {
  components: {
    Hello,
    test1,
    test3,
    test4,
    test5
  }
}
</script>

<style>
html {
  height: 100%;
}

body {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
}

#app {
  color: #2c3e50;

  max-width: 600px;
  font-family: Source Sans Pro, Helvetica, sans-serif;
  text-align: center;
}

#app a {
  color: #42b983;
  text-decoration: none;
}

.logo {
  width: 100px;
  height: 100px
}
</style>
