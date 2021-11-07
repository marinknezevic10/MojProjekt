<template>
  <div id="app">
    <h1>Fetching data with api</h1>
    <PopularMovies />
  </div>
</template>
<script>
import PopularMovies from "/components/PopularMovies";
export default {
  name: "App",
  components: {
    PopularMovies,
  },
};
</script>
