<template>
   <no-ssr>
      <vue-tiny-slider 
        :mouse-drag="false" 
        :loop="true"
        navPosition='bottom'
        :controls="sliderControls"
        :autoplayButtonOutput="false" 
        :items="sliderItem"
        :autoplay="sliderAutoPlay"
        >
         <slot></slot>
      </vue-tiny-slider>
    </no-ssr>
</template>

<script>
  export default {
      name: 'Slider',
      props:['sliderItem','sliderAutoPlay', 'sliderControls'],
      components: {
      },
       data(){
        return{
        }
      },
      computed:{
        MainSliders () {
          return this.$store.state.mainSlider.sliders
        }
      },
      mounted(){
      }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>



</style>
