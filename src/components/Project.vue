<template>
    <b-card-group deck>
        <project-item v-for="(repository,key) in repositories" :repository="repository" :key="key">
        </project-item>
    </b-card-group>
</template>

<script>
import ProjectItem from "./ProjectItem.vue";
export default {
  name: "project",
  data() {
    return {
      repositories: null
    };
  },
  components: {
    ProjectItem
  },
  beforeMount() {
    fetch("https://api.github.com/users/arielmikiabraham/repos")
      .then(res => res.json())
      .then(res => {
        this.repositories = res;
      })
      .catch(console.log);
  }
};
</script>

<style scoped>
.card-deck {
  display: flex;
  justify-content: center;
  flex-flow: row wrap;
  align-items: stretch;
}
.card-deck .card {
  display: block;
  flex-grow: 0;
  flex-basis: 22%;
  margin-bottom: 1rem;
}

@media screen and (max-width: 768px) {
    .card-deck .card {
        flex-basis: 100%;
    }
}
</style>


