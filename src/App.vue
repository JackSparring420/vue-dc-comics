<template>
  <div id="app">
    <Header/>
    <main>
      <Jumbotron/>
      <Comics/>
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
import Jumbotron from './components/Jumbotron.vue'
import NavByIcons from './components/NavByIcons.vue'
import FooterLinks from './components/FooterLinks.vue'
import FooterFollow from './components/FooterFollow.vue'
import Comics from './components/Comics.vue'

export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    NavByIcons,
    FooterLinks,
    FooterFollow,
    Comics
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
