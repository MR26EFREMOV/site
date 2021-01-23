<template>
  <div>
    <NavBar />
    <main>
      <Nuxt />
    </main>
  </div>
</template>

<script>
import NavBar from '../components/NavBar'

export default {
  components: {
    NavBar,
  },
}
</script>
