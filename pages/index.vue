<template>
  <section class="app">
    <Header/>
    <MainSlider/>
    <MainBlocks/>
  </section>
</template>

<script>
  import Header from '../containers/Header'
  import MainSlider from '../containers/MainSlider'
  import MainBlocks from '../containers/MainBlocks'
  export default {
    components: {
      Header,
      MainSlider,
      MainBlocks
    }
  }
</script>

<style>
  @import url('../styles/main.min.css');
</style>