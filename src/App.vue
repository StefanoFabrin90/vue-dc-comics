<template>
  <div id="app">
    <!-- header -->
    <Header />

    <!-- hero -->
    <Hero />

    <!-- main -->
    <main>
      <!-- section-content-1 -->
      <Section1 />

      <!-- section-content-2 -->
      <Section2 />
    </main>

    <!-- footer -->
    <footer>
      <!-- section-1 footer -->
      <Footer1 />

      <!-- section-2 footer -->
      <Footer2 />
    </footer>

  </div>
</template>

<script>
import Header from '@/components/Header.vue' 
import Section1 from '@/components/Section1.vue' 
import Section2 from '@/components/Section2.vue' 
import Footer1 from '@/components/Footer1.vue' 
import Footer2 from '@/components/Footer2.vue'
import Hero from '@/components/Hero.vue' 


export default {
  name: 'App',
  components: {
    Header,
    Section1,
    Section2,
    Footer1,
    Footer2,
    Hero,
  }
}
</script>

<style lang="scss">
  @import'@/styles/global.scss';
  @import'@/styles/Utilities.scss';

</style>
