<template>
  <div id="app">
        <H5_range></H5_range>
      <Range1></Range1> 
      <slider :min=1 :max=5 v-model = "per"></slider>
    <router-view/>
  </div>
</template>

<script>
  import H5_range from './components/h5 range.vue'
  import Range1 from './components/range1.vue'
  import slider from './pages/game28.vue'
  export default {
    data(){
      return {per:1}  
    },
    name: 'App',
    components: { Range1,slider,H5_range },
    created() {
     
    },
  }

</script>
<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>