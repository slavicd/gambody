<template>
  <div class="row">
    <div class="col-lg-6 col-12" v-for="(block, i) in featureBlocks" :key="i">
      <div class="main-blocks__item main-blocks_slider">
        <div class="main-blocks__title">
            {{block.title}}
        </div>
        <div 
          class="main-blocks__content main-blocks-slider slider-style-black"
          v-if="block.sliders"
          >
          <Slider 
            :sliderItem="items.item"
            :sliderAutoPlay="items.false"
            :sliderControls="items.sliderControls"
            >
            <div class="slider-two-rows__wrap"
                v-for="(slide, i) in block.sliders"
                :key="i"
              >
              <a :href="sl.href"
                class="slider-two-rows__item" 
                v-for="(sl, i) in slide.slide"
                :key="i"
                >
                  <div class="slider-two-rows__item-img">
                      <img src="@/img/png/main-blocks__slide1.png"
                        srcset="@/img/png/main-blocks__slide1@2x.png 2x,
                        @/img/png/main-blocks__slide1@3x.png 3x" alt="category">
                  </div>
                  <div class="slider-two-rows__title">{{sl.title}}</div>
              </a>
            </div>
          </Slider>
        </div>
        <div v-if="!block.sliders">
          <div class="main-blocks__content">
              <img
                src="@/img/jpg/main-block1.jpg"
                srcset="@/img/jpg/main-block1@2x.jpg 2x,
                @/img/jpg/main-block1@3x.jpg 3x" alt="main-blocks"
                >
          </div>
          <div class="main-blocks__description">
              {{block.description}}
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
    import Slider from '../MainSlider/Slider'
    export default {
      name: 'MainBlock',
      props:['featureBlocks', 'items'],
      components: {
        Slider
      },
      computed:{
      }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >

</style>
