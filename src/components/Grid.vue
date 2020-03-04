<template>
<div>
  <div class='grid-container row'>
      <tile class='col-3 tile' v-for="(tile, index) in tiles" :key="index" :tile="tile"></tile>
  </div>
</div>
</template>

<script>

import Tile from '../components/Tile.vue'

export default {
    data () {
      let tiles = []
      for (let i = 0; i < 16; i++) {
        tiles.push({score: ""})
      }
      console.log(tiles)
      return {
        tiles: tiles
      }
    },
    components: {
      Tile
    },
}
</script>



<style scoped>
    .grid-container {
        width: 440px; 
        height: 440px; 
        margin: auto;
        margin-top: 5px;
    }
    .tile {
      background: #2D2F3D;
      padding: 5px;
    }
</style>