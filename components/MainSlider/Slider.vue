<template>
   <div class="slider main-slider__block">
     <div class="main-slider__item" ><img  src="../../img/jpg/home_background.jpg"  alt="slider"/></div>
     <div class="main-slider__item" ><img  src="../../img/jpg/home_background.jpg" alt="slider"/></div>
     <div class="main-slider__item" ><img  src="../../img/jpg/home_background.jpg" alt="slider"/></div>
   </div>
</template>

<script>
  export default {
      name: 'Slider',
      components: {

      },
      data(){
        return{
        }
      },
      mounted(){
        let slider = document.querySelector('.main-slider__block');
          if(slider){
              tns({
                container: '.main-slider__block',
                items:1,
                nav: true,
                navPosition: 'bottom',
                controls: false,
                gutter:0,
                loop:true,
              autoplayButtonOutput:false,
                autoplay: true,
                responsive:{
                    750:{
                        controls: true,
                    },
                }
            });
          }
      }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>



</style>
