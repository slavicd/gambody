<template>
  <section class="main-blocks">
    <div class="container">
      <MainBlock :featureBlocks="featureBlocks" :items="optionsSlider"/>
    </div>
  </section>
</template>

<script>
    import MainBlock from '../components/MainBlocks/MainBlock'
    import Slider from '../components/MainSlider/Slider'
    export default {
        name: 'MainBlocks',
        components: {
          MainBlock,
          Slider
        },
         data(){
          return{
            featureBlocks:[
              {
                title: 'title',
                description:'description',
                sliders:[
                  {
                    slide:[
                      {
                        href:'',
                        img:'',
                        title:'title',
                      },
                      {
                        href:'',
                        img:'',
                        title:'title2',
                      },
                      
                    ]
                  },
                  {
                    slide:[
                      {
                        href:'',
                        img:'',
                        title:'title',
                      },
                      {
                        href:'',
                        img:'',
                        title:'title2',
                      }
                    ]
                  },
                  {
                    slide:[
                      {
                        href:'',
                        img:'',
                        title:'title',
                      },
                      {
                        href:'',
                        img:'',
                        title:'title2',
                      }
                    ]
                  },
                  {
                    slide:[
                      {
                        href:'',
                        img:'',
                        title:'title',
                      },
                      {
                        href:'',
                        img:'',
                        title:'title2',
                      }
                    ]
                  },
                  

                ]
              },
              {
                title: 'title',
                slider:false,
                description:'description'
              },

            ],
            optionsSlider:{
              item: 3,
              autoPlay:false,
              sliderControls:true
            }
          }
        },
        mounted(){
          if(window.innerWidth <= 578){
            this.items.item = 2;
            this.sliderControls = false
          }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  #tns2-ow{
    width: 120% !important;
  }
  @media screen and (max-width: 578px) {
    #tns2-ow{
      width: 100% !important;
    }
  }
    #tns3-ow{
    width: 120% !important;
  }
  @media screen and (max-width: 578px) {
    #tns3-ow{
      width: 100% !important;
    }
  }
</style>


