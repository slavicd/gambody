<template>
 <div class="topline header__inner">
   <div class="topline__container">
     <nav class="menuflat topline__menu">
       <ul class="menuflat__list" >
        <li :class="list.ulDropDown ? 'menuflat__item' + ' ' +  list.classLi : 'menuflat__item' "
         v-for="(list, i) in menuflatList" :key="i"
         >
            <a :href="list.link"
             :class="list.ulDropDown ? 'link menuflat__link' + ' ' +  list.classLink : 'link menuflat__link' "
              >
              {{list.textLink}}
            </a>
            <ul class="dropdown dropdown-content" v-if="list.ulDropDown">
                <li class="menu-arrow"></li>
                <li class="menuflat__item" v-for="(listDropDown, i) in list.ulDropDown" :key="i">
                    <a :href="listDropDown.link" class="link menuflat__link color_black">{{listDropDown.textLink}}</a>
                </li>
            </ul>
        </li>
       </ul>
     </nav>
     <div class="socialflat topline__social">
      <a href="javascript:;"
        :class="'socialflat__item' + ' ' + link.classLink" v-for="(link, i) in socialflat"
        :key="i"
        >
      </a>
     </div>
     <div class="menuflat langflat topline__lang">
       <ul class="menufl at__list">
          <li class="menuflat__item dropdown menuflat_dropdown">
              <a href="#" class="link menuflat__link langflat__link">
                  <img src="../../img/png/en.png" srcset="../../img/png/en@2x.png 2x, ../../img/png/en@3x.png 3x" alt="langflat__link_en"></a>
              <ul class="dropdown dropdown-content">
                  <li class="menu-arrow"></li>
                  <li class="menuflat__item">
                      <a href="#" class="link menuflat__link langflat__link">
                          <img src="../../img/png/en.png" srcset="img/png/en@2x.png 2x, img/png/en@3x.png 3x" alt="langflat__link_en"></a>
                  </li>
              </ul>
          </li>
       </ul>
     </div>
     <div class="menuflat currency topline__currency">
           <ul class="menuflat__list">
               <li class="menuflat__item dropdown menuflat_dropdown">
                   <a href="#" class="link menuflat__link currency__link">USD</a>
                   <ul class="dropdown dropdown-content">
                       <li class="menu-arrow"></li>
                       <li class="menuflat__item">
                           <a href="#" class="link menuflat__link currency__link">USD</a>
                       </li>
                       <li class="menuflat__item">
                           <a href="#" class="link menuflat__link currency__link">EUR</a>
                       </li>
                   </ul>
               </li>
           </ul>
     </div>
   </div>
 </div>
</template>

<script>
export default {
  data(){
   return{

   }
  },
  computed:{
     menuflatList () {
       return this.$store.state.header.menuflatList
    },
    socialflat () {
       return this.$store.state.header.socialflat
    }


  //  menuflatList(){
  //    return this.$store.getters.menuflatList
  //  },
  //  socialflat(){
  //   return this.$store.getters.socialflat
  //  }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >

</style>
