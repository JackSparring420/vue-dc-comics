<template>
  <div id="app">
    <Header/>
    <main>
      <Main/>
    </main>
    <footer>
      <NavByIcons/>
      <FooterLinks/>
      <FooterFollow/>
    </footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import NavByIcons from './components/NavByIcons.vue'
import FooterLinks from './components/FooterLinks.vue'
import FooterFollow from './components/FooterFollow.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    NavByIcons,
    FooterLinks,
    FooterFollow
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box; 
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 50px;
}

</style>
