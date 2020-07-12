<template>
  <section class="app">
   <Header/>
   <MainSlider/>
  </section>
</template>

<script>
import Header from '../containers/Header'
import MainSlider from '../containers/MainSlider'
export default {
  components: {
    Header,
    MainSlider
  }
}
</script>

<style>
@import url('../styles/main.min.css');

</style>

