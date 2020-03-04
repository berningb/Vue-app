<script>
  export default {
    props: ['circle'],
    computed: {
      style () {
        return 'background-color: ' + this.circle.color;
      }
    },
    components: { 
    }
  }
</script>

<template>
 <div id="circle" :style="style">
   {{circle.name}}
 </div>
</template>

<style scoped>
   #circle {
        border-radius: 100px;
        width: 100px;
        height: 100px;
    }
</style>