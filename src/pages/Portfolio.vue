<template>
<div>
  <main-layout></main-layout>
  <div class="container-fluid row" style="margin: auto">
    <project class="col-3" v-for="(proj, index) in projects" :key="index" :project="proj"></project>
  </div>
</div>
</template>

<script>
  import MainLayout from '../layouts/Nav.vue'
  import Project from '../components/Project.vue'

  export default {
    components: {
      MainLayout,
      Project
    },
    data () {
      let projects = []
      for (let i = 0; i < 10; i++) {
        projects.push({name: 'Project ' + i})
      }
      return {
        projects
      }
    }
  }
</script>
