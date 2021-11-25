<template>
    <div class="comic">
        <div class="contain-img"><img :src="details.thumb" :alt="details.series"></div>
        <h4>{{details.series}}</h4>
    </div>
</template>

<script>
export default {
  name: 'Comic',
  props: {
      details:Object
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .comic {
    width: calc(100% / 6);
    margin-bottom: 20px;
    
    h4 {
        color: white;
        width: 150px;
        margin: 10px 0;
    }

    .contain-img {
        width: 150px;
        height: 150px;

        img{
           object-fit: cover;
           object-position: 0 10px;
           width: 100%;
           height: 100%; 
        }
    } 
  }
</style>