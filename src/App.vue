<template>
  <div>
    <Welcome/>
    <Project class="my-4 mx-auto" />
  </div>
</template>

<script>
import Welcome from "./components/Welcome.vue";
import Project from "./components/Project.vue";
export default {
  name: "app",
  data() {
    return {
      isLoading: true
    };
  },
  components: {
    Welcome,
    Project
  }
};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Lato");
@import url("https://use.fontawesome.com/releases/v5.0.13/css/all.css");
* {
  font-family: "Lato", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0 0;
}

h1,
h2 {
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
</style>
