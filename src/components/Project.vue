<template>
<div style="padding: 10px" v-on:click="say(project)">
    <div id='box'>
      <h3 style="text-align: center">
        {{project.name}}  
      </h3>
    </div>
</div>
</template>

<script>
  export default {
    components: {
    },
    methods: {
      say: function (message) {
        console.log(message)
      }
    },
    props: ['project']
  }
</script>

<style scoped>
    #box {
        border: 1px solid black;
        width: 100%;
        height: 300px;
        border-radius: 3px;
    }

</style>
