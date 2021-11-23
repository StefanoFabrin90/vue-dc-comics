<template>
  <div id="app">
    <!-- header -->
    <Header />

    <!-- main -->
    <main>
      <!-- section-content-1 -->
      <Section1 />
      

    </main>

  </div>
</template>

<script>
import Header from '@/components/Header.vue' 
import Section1 from '@/components/Section1.vue' 


export default {
  name: 'App',
  components: {
    Header,
    Section1,
  }
}
</script>

<style lang="scss">
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: sans-serif;
  }

  img {
    max-width: 100%;
  }

  // utilities
.container {
  max-width: 1170px;
  margin: 0 auto;
  padding: 0 16px;
}

.display-flex {
  display: flex;
}

.justify-content {
  justify-content: space-between;
}
</style>
