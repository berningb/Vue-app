<template>
<div id='grid-wrapper'>
    <div style="width: 450px; margin:auto;">
        <p style="font-size: 3em; font-weight: bold; margin: 0">2048</p>
        <div style="overflow: auto">
            <div style="float: right; display: flex">
                <div class='score mini-box'>
                    <p class="m-0">SCORE</p>
                    <p class="m-0">{{score}}</p>
                </div>
                <div class="best-score mini-box">
                    <p class="m-0">BEST SCORE</p>
                    <p class="m-0">{{bestScore}}</p>
                 </div>
            </div>
        </div>
    </div>
  <div id='grid' style="margin:auto; marginTop :20px; padding-top: 1px">
      <grid></grid>
  </div>
</div>
</template>

<script>
    import Grid from '../components/Grid.vue'

    export default {
        components: {
            Grid
        },
        data () {
            return {
                score: 0,
                bestScore: 0
            }
        },
    }
</script>



<style scoped>
#grid {
    background: #2D2F3D;
    border-radius: 10px;
    height: 450px;
    width: 450px
}
#grid-wrapper {
    margin-top: 20px;
    background: #20212C;
}
.mini-box {
    width: auto;
    color: white;
    background: #43465A;
    border-radius: 10px;
    margin: 10px;
    text-align: center;
    font-weight: bold;
    font-size: 16px;
    padding: 5px 10px 5px 10px;
}
.clear {
     clear: both;   
};
.m-0 {
    margin: 0
}
</style>