<template>
  <div id='bob'>
      <game-grid></game-grid>
  </div>
</template>

<script>
import GameGrid from '../components/GridWrapper.vue'

  export default {
    components: {
      GameGrid
    }
  }
</script>



<style scoped>
#bob {
    background: #20212C;
    height: 100%;
    color: white
}
</style>