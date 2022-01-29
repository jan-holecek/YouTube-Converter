<template>
  <Navbar></Navbar>
  <Head></Head>
  <About></About>
  <div class="background">
  <HowTo></HowTo>
  </div>
  <Footer></Footer>
</template>

<script>
import Head from '@/components/Head.vue'
import Navbar from '@/components/Navbar.vue'
import HowTo from '@/components/HowTo.vue'
import About from '@/components/About.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'Home',
  components: {
    Head,
    Navbar,
    HowTo,
    About,
    Footer
  }
}
</script>

<style scoped>
.background {
  background: #28363A;
  margin-top: 50px;
}
</style>