<template>
  <div id="app">
    <img class="center" src="./assets/logo.png">
    <h1>{{ title }}</h1>
    <Navbar />
    <Blogs />
  </div>
</template>

<script>
import Navbar from './Navbar'
import Blogs from './Blogs'
export default {
  name: 'app',
  components: {
    Navbar,
    Blogs
  },
  data () {
    return {
      title:'My first Vue app',

    }
  },
  methods: {

  }
}
</script>

<style>
h1{
  color: #444;
  font-weight: normal;
  text-align: center;
}

.center{
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 10%;
}

</style>
