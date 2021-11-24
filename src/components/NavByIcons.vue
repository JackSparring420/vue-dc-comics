<template>
    <footer>
        <nav>
            <ul>
                <li v-for="link, i in links" :key="i">
                    <a :href="link.url" >
                        <span class="icon"><img :src="link.icon" :alt="link.text"></span>
                        <span>{{link.text}}</span>
                    </a>
                </li>
            </ul>
        </nav>
    </footer>
</template>

<script>
export default {
  name: 'Header',
  data() {
      return {
          links: [
              {
                  text: "DIGITAL COMICS",
                  url: "#",
                  icon: "assets/img/buy-comics-digital-comics.png",
              },
              {
                  text: "DC MERCHANDISE",
                  url: "#",
                  icon: "assets/img/buy-comics-merchandise.png",
              },
              {
                  text: "SUBSCRIPTION",
                  url: "#",
                  icon: "assets/img/buy-comics-subscriptions.png",
              },
              {
                  text: "COMIC SHOP LOCATOR",
                  url: "#",
                  icon: "assets/img/buy-comics-shop-locator.png",
              },
              {
                  text: "DC POWER VISA",
                  url: "#",
                  icon: "assets/img/buy-dc-power-visa.svg",
              },
          ]
      }
  },
  methods: {
      
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
        footer {
        background-color: #0282f9;
        height: 200px;
        display: flex;
        align-items: center;
            nav{
                width: 70%;
                margin: auto;
                
                ul {
                    display: flex;
                    justify-content: space-between;
                    list-style-type: none;
                        a {
                            display: flex;
                            align-items: center;
                            text-decoration: none;
                            color: white;
                                .icon{
                                    display: inline-block;
                                    width: 70px;
                                    height: 70px;
                                    margin-right: 10px;
                                }
                                img {
                                    object-fit: contain;
                                    width: 100%;
                                    height: 100%;
                                }
                        }
                }
            }
    }
</style>
