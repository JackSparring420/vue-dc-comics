<template>
    <footer>
        <div id="contain">
        <nav id="links">
            <div>
                <ul>
                    <h3>DC COOMICS</h3>
                    <li v-for="comic, i in comics" :key="i">
                        <a :href="comic.url">{{comic.text}}</a>
                    </li>
                </ul>
                <ul>
                    <h3>SHOP</h3>
                    <li v-for="comic, i in shop" :key="i">
                        <a :href="comic.url">{{comic.text}}</a>
                    </li>
                </ul>

            </div>
            <ul>
                <h3>DC</h3>
                <li v-for="link, i in dc" :key="i">
                    <a :href="link.url">{{link.text}}</a>
                </li>
            </ul>
            <ul>
                <h3>SITES</h3>
                <li v-for="link, i in sites" :key="i">
                    <a :href="link.url">{{link.text}}</a>
                </li>
            </ul>
        </nav>
        <div id="logo">
            <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
        </div>
    </footer>
</template>

<script>
export default {
  name: 'Header',
  data() {
      return {
          comics: [
              {
                  text: "Character",
                  url: "#",
              },
              {
                  text: "Comics",
                  url: "#",
              },
              {
                  text: "Movie",
                  url: "#",
              },
              {
                  text: "TV",
                  url: "#",
              },
              {
                  text: "Games",
                  url: "#",
              },
              {
                  text: "Videos",
                  url: "#",
              },
              {
                  text: "News",
                  url: "#",
              }
          ],
          dc: [
              {
                  text: "Terms Of Use",
                  url: "#",
              },
              {
                  text: "Privacy policy (New)",
                  url: "#",
              },
              {
                  text: "Ad Choise",
                  url: "#",
              },
              {
                  text: "Advertising",
                  url: "#",
              },
              {
                  text: "Jobs",
                  url: "#",
              },
              {
                  text: "Subscrictions",
                  url: "#",
              },
              {
                  text: "Talent Workshops",
                  url: "#",
              },
              {
                  text: "CPSC Certificates",
                  url: "#",
              },
              {
                  text: "Ratins",
                  url: "#",
              },
              {
                  text: "Shop Help",
                  url: "#",
              },
              {
                  text: "Contact Us",
                  url: "#",
              }
          ],
          sites:[
              {
                  text: "DC",
                  url: "#",
              },
              {
                  text: "MAD Magazine",
                  url: "#",
              },
              {
                  text: "DC Kids",
                  url: "#",
              },
              {
                  text: "DC Universe",
                  url: "#",
              },
              {
                  text: "DC Power Visa",
                  url: "#",
              }
          ],
          shop: [
              {
                  text: "Shop DC",
                  url: "#",
              },
              {
                  text: "Shop DC Collectibles",
                  url: "#",
              }
          ]
      }
  },

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    footer {
        background-image: url("../assets/img/footer-bg.jpg");
        background-size: cover;
        align-items: center;

            #contain {
                display: flex;
                justify-content: space-between;
                align-items: center;
                width: 70%;
                margin: auto;
                justify-content: space-between;

                nav {
                    display: flex;
                    justify-content: space-between;
                }

                #links{
                    width: 50%;
                }

                #logo {
                    margin-right: 100px;
                    width: 50%;
                    height: 350px;
                    
                    img {
                    object-fit: none;
                    width: 150%;
                    height: 100%;
                    }
                }

                ul {
                    list-style-type: none;
                    margin: 30px 30px 0;


                    h3 {
                        color: white;
                        margin-bottom: 15px;
                    }
        
                    a {
                        color: gray;
                        text-decoration: none;
                    }
                }
            }
        }
</style>
