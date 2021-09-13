<template>
 <div class="blogs">
  <h2>{{blogTitle}}</h2>
  <button @click="changeTitle">Change Title</button>
 </div>
</template>

<script>
import Navbar from './Navbar'

export default {
  name: 'Blogs',
  data() {
    return {
      blogTitle:'Blogs',
    }
  },
  methods:{
    changeTitle(){
      this.blogTitle = 'Amazing Blog Site'
    }
  },
  beforeCreate(){
    alert('BeforeCeate hook')
  },
  created(){
    alert('Created hook')
  },
  beforeUpdate(){
    alert('BeforeUpdate hook')
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
