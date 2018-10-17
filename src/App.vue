<template>
  <div id="app">
    <div class="container">
      <wedding-header>
      </wedding-header>
    </div>
    <div class="container">
      <router-view></router-view>
    </div> 
    <div class="container">
      <wedding-footer>
      </wedding-footer>
    </div>
    </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Home from './components/Footer.vue'

export default {
  components: {
    weddingHeader: Header,
    weddingFooter: Footer,
  },
}
</script>

<style>

</style>
