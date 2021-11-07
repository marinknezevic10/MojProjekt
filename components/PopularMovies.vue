<template>
  <div>
    <h1>Popular Movies</h1>
    <tbody>
    <tr v-for="popularmovie in popularmovies" v-bind:key="popularmovie.id">
      <th>{{popularmovie.id}}</th>
    </tr>
    </tbody>
  </div>
</template>
<script>
import axios from 'axios';

export default {
  name: 'PopularMovies',
  data(){
    return {
      popularmovies: null,
    };
  },
  created: function() {
    axios
      .get('https://www.themoviedb.org/movie')
      .then(res=> {
        this.popularmovies = res.data;
      })
  }

}
</script>
