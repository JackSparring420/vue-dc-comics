<template>
    <header>
        <img src="../assets/img/dc-logo.png" alt="">
        <nav>
            <ul>
                <li v-for="link, i in links" :key="i">
                    <a :href="link.url" :class="link.here? 'active' : ''"><strong>{{link.text}}</strong></a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
      return {
          links: [
              {
                  text: "CHARACTER",
                  url: "#",
                  here: false,
              },
              {
                  text: "COMICS",
                  url: "#",
                  here: true,
              },
              {
                  text: "MOVIES",
                  url: "#",
                  here: false,
              },
              {
                  text: "TV",
                  url: "#",
                  here: false,
              },
              {
                  text: "GAMES",
                  url: "#",
                  here: false,
              },
              {
                  text: "COLLECTIBLES",
                  url: "#",
                  here: false,
              },
              {
                  text: "VIDEOS",
                  url: "#",
                  here: false,
              },
              {
                  text: "FANS",
                  url: "#",
                  here: false,
              },
              {
                  text: "NEWS",
                  url: "#",
                  here: false,
              },
              {
                  text: "SHOP",
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
    header {
        width: 70%;
        margin: auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        li {
            display: inline-block;
            margin: 0 10px;

            a {
                color: black;
                text-decoration: none;
                padding-bottom: 50px;
                &.active {
                    color: #0282f9;
                    border-bottom: #0282f9 5px solid;
                }
            }
        }
    }
</style>
