<template>
    <main>
        <div class="contain">
            <strong>CURRENT SERIES</strong> 
        </div>
    </main>
</template>

<script>
export default {
  name: 'Header',
  data() {
      return {
      }
  },
//   methods(){

//   }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    main {
        padding: 0;
        margin: 12px 0 0 0;
        box-sizing: border-box;
        background-image: url("../assets/img/jumbotron.jpg");
        display: flex;
        align-items: center;
        height: 435px;
        position: relative;
            .contain{
                position: absolute;
                background-color: #0282f9;
                padding: 5px 10px;
                color: white;
                top: 420px;
                left: 15%;
            }
    }
</style>
