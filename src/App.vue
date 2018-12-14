<template>
  <div id="app">
    <Header title="California Title 24 Reports"/>
    <!-- 
      Old Logo
      <img alt="Vue logo" src="./assets/logo.png"> 
    -->
    <Landing title="Welcome to California Title 24 Reports" />
    <div v-show="showContact">
      <Contact />
    </div>
    <Footer title="Footer"/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
// import Posts from './components/Posts.vue'
import Contact from './components/Contact.vue'
import Landing from './components/Landing.vue'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

export default {
  name: 'app',
  data () {
    return {
      showContact: true
    }
  },
  components: {
    Header,
    Footer,
    Contact,
    Landing
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
