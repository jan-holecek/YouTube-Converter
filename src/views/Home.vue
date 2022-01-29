<template>
  <Navbar></Navbar>
  <Head></Head>
  <About></About>
  <div class="background">
  <HowTo></HowTo>
  </div>
</template>

<script>
import Head from '@/components/Head.vue'
import Navbar from '@/components/Navbar.vue'
import HowTo from '@/components/HowTo.vue'
import About from '@/components/About.vue'

export default {
  name: 'Home',
  components: {
    Head,
    Navbar,
    HowTo,
    About,
  }
}
</script>

<style scoped>
.background {
  background: #28363A;
  margin-top: 50px;
}
</style>
