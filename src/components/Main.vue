<template>
    <main>
        <div class="contain">
            <h2> --&gt; Content goes here &lt;-- </h2>
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
        background-color: black;
        display: flex;
        align-items: center;
        height: 200px;
            .contain{
                width: 70%;
                margin: auto;
                
                h2 {
                    color: white;
                }
            }
    }
</style>
