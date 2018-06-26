<template>
  <div class="hello">
    <header-bar></header-bar>
    <div class="main">
      <asid-bar></asid-bar>
      <sections></sections>
    </div>
    
  </div>
 
</template>

<script>
  import headerBar from './headerBar'
  import asideBar from './asideBar'
  import sections from './section'
export default {
  name: 'homePage',
  components: {
    "header-bar": headerBar,
    "asid-bar": asideBar,
    "sections": sections
  },
  data () {
    return {
    }
  }
}
</script>

<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.hello{
  background: #f2f2f2;
}

.main{
  width: 80%;
  height:780px;
  margin: 15px auto 0;
  background: #f2f2f2;
  display: flex;
}
</style>
