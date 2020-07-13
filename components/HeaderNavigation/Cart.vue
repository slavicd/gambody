<template>
 <div>
   <div class="add-btn main-header__button-type">
     <div class="add-btn__item main-header_btn">
     </div>
   </div>
   <div class="main-header__mixblocks">
     <div class="account-block main-header__account">
         <div class="account-block__item main-header_btn dropdown" aria-haspopup="true">
             <a href="javascript:;" class="mob-link"></a>
             <div class="account-block__wrap">
                 <img src="../../img/jpg/user-picture-premium.jpg" srcset="../../img/jpg/user-picture-premium@2x.jpg 2x, ../../img/jpg/user-picture-premium@3x.jpg 3x" alt="account">
                 <div class="account-block__content">
                     <div class="account-block__name">
                         Hello, <span>Massimiliano</span>
                     </div>
                     <div class="account-block__balance">
                         $1201.50
                     </div>
                 </div>
             </div>
             <ul class="dropdown dropdown-content account-block__dropdown">
                 <li class="menu-arrow"></li>
                 <li class="">
                     <a href="#" class="link dropdown-content__link color_black">Profile</a>
                 </li>
                 <li class="">
                     <a href="#" class="link dropdown-content__link color_black">Shop</a>
                 </li>
                 <li class="">
                     <a href="#" class="link dropdown-content__link color_black">Favourites</a>
                 </li>
                 <li class="">
                     <a href="#" class="link dropdown-content__link color_black">Purchases</a>
                 </li>
                 <li class="">
                     <a href="#" class="link dropdown-content__link color_black"><span>Earned</span><div class="dropdown__count">21</div></a>
                 </li>
                 <li class="dropdown__line"></li>
                 <li class="">
                     <a href="#" class="link dropdown-content__link color_black">Log out</a>
                 </li>
             </ul>
         </div>
       </div>

       <div class="mini-cart main-header__button-wrap">
           <div class="mini-cart__wrap dropdown" aria-haspopup="menu">
               <a href="javascript:;" class="mob-link"></a>
           <div class="mini-cart__item main-header_btn">
               <div class="mini-cart__count">10</div>
           </div>
           <div class="dropdown dropdown-content">
               <div class="menu-arrow"></div>
               <ul>
               <li class="mini-cart__li">
                   <a href="#" class="link mini-cart__link">
                       <img src="img/png/mini-cart-img1.png" alt="product">
                       <div class="mini-cart__content">
                           <div class="mini-cart__title">Jaina 3D Printing Figurine | Assembly</div>
                           <div class="mini-cart__type"><span>Type:</span>FDM, SLA/DLP, SLS</div>
                       </div>
                       <div class="mini-cart__price">
                           $29.95
                       </div>
                   </a>
               </li>
               <li class="mini-cart__li">
                       <a href="#" class="link mini-cart__link">
                           <img src="img/png/mini-cart-img2.png" alt="product">
                           <div class="mini-cart__content">
                               <div class="mini-cart__title">Pennywise Clown from "IT" 3D Printing Miniature | Assembly</div>
                               <div class="mini-cart__type"><span>Type:</span>FDM, SLA/DLP, SLS</div>
                           </div>
                           <div class="mini-cart__price">
                               $29.95
                           </div>
                       </a>
               </li>
                   <li class="mini-cart__li">
                       <a href="#" class="link mini-cart__link">
                           <img src="img/png/mini-cart-img3.png" alt="product">
                           <div class="mini-cart__content">
                               <div class="mini-cart__title">Jaina 3D Printing Figurine | Assembly</div>
                               <div class="mini-cart__type"><span>Type:</span>FDM, SLA/DLP, SLS</div>
                           </div>
                           <div class="mini-cart__price">
                               $29.95
                           </div>
                       </a>
                   </li>
                   <li class="mini-cart__li">
                       <a href="#" class="link mini-cart__link">
                           <img src="img/png/mini-cart-img4.png" alt="product">
                           <div class="mini-cart__content">
                               <div class="mini-cart__title">Jaina 3D Printing Figurine | Assembly</div>
                               <div class="mini-cart__type"><span>Type:</span>FDM, SLA/DLP, SLS</div>
                           </div>
                           <div class="mini-cart__price">
                               $29.95
                           </div>
                       </a>
                   </li>
               </ul>


               <div class="mini-cart__footer">
                   <div class="mini-cart__footer-title">You have 4 items in  your shopping cart</div>
                   <div class="dropdown__line"></div>
                   <div class="mini-cart__total">
                       <div class="mini-cart__total-title">
                           Total:
                       </div>
                       <div class="mini-cart__total-price">
                           $255.95
                       </div>
                   </div>
                   <div class="mini-cart__btns">
                       <a href="#" class="link button button_secondary button_m">View cart</a>
                       <a href="#" class="link button button_primary button_m">To Checkout</a>
                   </div>

               </div>
           </div>
           </div>
       </div>
   </div> <!-- mobile block -->
 </div>
</template>

<script>
export default {
  data(){
   return{

   }
  },
  computed:{
 
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >

</style>
