<template>
  <div id="viewDiv">
    <el-button v-text="buttonName"></el-button>
  </div>
</template>

<script>
import Vue from 'vue'
import esriLoader from 'esri-loader'
import Button from 'element-ui'
Vue.use(Button)

export default {
  name: 'HelloWorld',

  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      buttonName: 'aaa'
    }
  },
  methods: {
    createMap () {
    }
  },
  mounted () {
    console.log(esriLoader.isLoaded())
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
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
  #viewDiv {
    width: 100%;
    height: 100%;
  }
</style>
