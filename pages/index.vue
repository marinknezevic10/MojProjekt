<template>
  <div id="app">
    <h1>Fetching data with api</h1>
    <PopularMovies />
  </div>
</template>
<script>
import PopularMovies from "../components/PopularMovies";
export default {
  name: "App",
  components: {
    PopularMovies,
  },
};
</script>

<style>
#app{
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    font-size: 2rem;
    margin-top: 60px;
}
</style>
