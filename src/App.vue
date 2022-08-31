<script>
import NavBar from './components/NavBar.vue'
import SlideShow from './components/SlideShow.vue'
import WebShoes from './components/WebShoes.vue'
import BandSection from './components/BandSection.vue'
import PageTour from './components/PageTour.vue'
import Contact from './components/Contact.vue'

export default {
  data() {
    return {
      page: "home"
    }
  },
  components: {
    NavBar,
    SlideShow,
    WebShoes,
    BandSection,
    PageTour,
    Contact
  },
  methods: {
    loadPage(page) {
      this.page = page
    }
  }
}
</script>

<template>
  <header>
    <NavBar page="setPage"/>
  </header>

  <main class="w3-content" style="max-width:2000px;margin-top:46px">
    <SlideShow v-if="page == 'home'"/>
    <BandSection v-if="page == 'band'" />
    <PageTour v-if="page == 'tour'" />
    <Contact v-if="page == 'contact'" />
  </main>

  <footer>
    <WebShoes />
  </footer>
</template>

<style scoped>
</style>
