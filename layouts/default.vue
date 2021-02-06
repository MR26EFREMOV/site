<template>
  <div>
    <NavBar />
    <v-main>
      <Nuxt />
    </v-main>
    <Footer />
  </div>
</template>

<script>
import NavBar from '../components/common/NavBar'
import Footer from '../components/common/Footer'

export default {
  components: {
    NavBar,
    Footer,
  },
}
</script>
