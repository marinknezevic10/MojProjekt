<template>
  <div>
    <h1>Popular Movies</h1>
  </div>
</template>
<script>
import Vue from 'vue';
import axios from 'axios'
import VueAxios from 'vue-axios'
Vue.use(VueAxios,axios)

export default {
  name: "PopularMovies",
  mounted()
  {
    Vue.axios.get('https://www.themoviedb.org/movie')
    .then((response)=>{
      console.warn(response)
    })
  }
};
</script>
