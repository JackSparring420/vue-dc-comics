<template>
    <footer>
        <div id="container">
        <button>SING-UP NOW!</button>
        <div>
            <ul>
                <h3>FOLLOW US</h3>
                <li v-for="icon, i in iconsFollow" :key="i">
                    <a :href="icon.url"><img :src="icon.icon" alt=""></a>
                </li>
            </ul>
        </div>
        </div>
    </footer>
</template>

<script>
export default {
  name: 'Header',
  data() {
      return {
          iconsFollow: [
              {
                  icon: "assets/img/footer-facebook.png",
                  url: "#",
                  here: false,
              },
              {
                  icon: "assets/img/footer-twitter.png",
                  url: "#",
                  here: true,
              },
              {
                  icon: "assets/img/footer-youtube.png",
                  url: "#",
                  here: false,
              },
              {
                  icon: "assets/img/footer-pinterest.png",
                  url: "#",
                  here: false,
              },
              {
                  icon: "assets/img/footer-periscope.png",
                  url: "#",
                  here: false,
              }
          ]
      }
  },

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    footer {
        background-color: #303030;
        display: flex;
        align-items: center;
        padding: 5px;

        #container {
            width: 70%;
            margin: auto;
            display: flex;
            justify-content: space-between;
            align-items: center;

            button {
                background-color: #303030;
                color: white;
                padding: 10px;
                border: solid 2px #0282f9;
            };

            ul {   
              display: flex;
              align-items: center;

                h3{
                    color: #0282f9;
                };

                li{
                    display: inline-block;
                    margin: 0 10px;
                }  
            };
        }
    }
</style>
