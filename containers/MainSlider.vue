<template>
  <section class="main-slider">
    <Slider    
      :sliderItem="1"
      :sliderAutoPlay="true"
      :sliderControls="sliderControls"
      >
      <div class="main-slider__item" v-for="(slider, i) in MainSliders" :key="i">
        <img src="@/img/jpg/home_background.jpg"  alt="slider"/>
      </div>
    </Slider>
  </section>
</template>

<script>
   import Slider from '../components/MainSlider/Slider'
    export default {
      name: 'MainSlider',
      components: {
          Slider
      },
      data(){
        return{
          sliderControls:true
        }
      },
      computed:{
        MainSliders () {
          return this.$store.state.mainSlider.sliders
        }
      },
      mounted(){
         if(window.innerWidth <= 578){
            this.sliderControls = false
          }
      }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >

</style>
