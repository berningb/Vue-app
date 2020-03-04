<template>
<div>
  <div class='b'>
      {{tile.score}}
  </div>
</div>
</template>

<script>
 export default {
    props: ['tile']
 }
</script>



<style scoped>
.b {
    border-radius: 5px;
    background: #43465A;
    width: 98%;
    height: 98%;
}
</style>