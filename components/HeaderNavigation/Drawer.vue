<template>
  <div class="menu hamburger-menu main-header__menu"> 
      <input id="menu__toggle" type="checkbox" />
      <label class="menu__btn main-header_btn" for="menu__toggle">
          <span></span>
      </label>

      <div class="menu__box main-nav">
          <label class="menu__btn menu__box-close" for="menu__toggle">
              <span></span>
          </label>
          <div class="main-nav__account">
              <img src="../../img/jpg/user-picture-premium.jpg" srcset="img/jpg/user-picture-premium@2x.jpg 2x, img/jpg/user-picture-premium@3x.jpg 3x" alt="account">
              <div>Hello,<span>Maverik</span> </div>
          </div>
          <div class="main-nav__menus">
              <ul class="main-nav__simple-menu">
                  <li><a class="main-nav__item" href="#">Popular</a></li>
                  <li><a class="main-nav__item" href="#">All items</a></li>
                  <li><a class="main-nav__item main-nav_special" href="#">Special deals</a></li>
              </ul>
              <div class="main-nav__category">
                  <div class="main-nav__title">
                      SHOP BY CATEGORY
                  </div>

                  <nav>
                    <div class="nav-level">
                        <ul>
                            <li class="multilevel">
                                <a href="javascript:;" class="back-icon main-nav__item">Anime</a>
                                <div class="multilevel-icon"></div>
                                <div class="submenu nav-level">
                                    <div class="back main-nav-cat-btn main-nav__item">Anime</div>
                                    <ul>
                                        <li><a href="#" class="back-icon main-nav__item">Level 2</a></li>
                                        <li><a href="#" class="back-icon main-nav__item">Level 2</a></li>
                                        <li><a href="#" class="back-icon main-nav__item">Level 2</a></li>
                                    </ul>
                                </div>
                            </li>
                            <li class="multilevel">
                                <a href="#" class="back-icon main-nav__item">Batman</a>
                                <div class="multilevel-icon"></div>
                                <div class="submenu nav-level">
                                    <div class="back back-icon main-nav__item">Batman</div>
                                    <ul>
                                        <li class="multilevel">
                                            <a href="#" class="back-icon main-nav__item">Level 2</a>
                                            <div class="multilevel-icon"></div>
                                            <div class="submenu nav-level">
                                                <div class="back back-icon main-nav__item">Level 2</div>
                                                <ul>
                                                    <li class="multilevel">
                                                        <a href="#" class="back-icon main-nav__item">Level 3</a>
                                                        <div class="multilevel-icon"></div>
                                                        <div class="submenu nav-level">
                                                            <div class="back back-icon main-nav__item">Level 3</div>
                                                            <ul>
                                                                <li><a href="#" class="back-icon main-nav__item">Level 4</a></li>
                                                                <li><a href="#" class="back-icon main-nav__item">Level 4</a></li>
                                                                <li><a href="#" class="back-icon main-nav__item">Level 4</a></li>
                                                            </ul>
                                                        </div>
                                                    </li>
                                                    <li><a href="#" class="back-icon main-nav__item">Level 3</a></li>
                                                    <li><a href="#" class="back-icon main-nav__item">Level 3</a></li>
                                                </ul>
                                            </div>
                                        </li>
                                        <li><a href="#" class="back-icon main-nav__item">Level 2</a></li>
                                        <li><a href="#" class="back-icon main-nav__item">Level 2</a></li>
                                        <li><a href="#" class="back-icon main-nav__item">Level 2</a></li>
                                    </ul>
                                </div>
                            </li>
                            <li><a href="#" class="back-icon main-nav__item">Cartoon</a></li>
                            <li><a href="#" class="back-icon main-nav__item">DC</a></li>
                            <li><a href="#" class="back-icon main-nav__item">Diorama</a></li>
                        </ul>
                    </div>
                  </nav>
              </div>
              <div class="main-nav__category">
                  <div class="main-nav__title">
                      HELP & ACCOUNT
                  </div>
                  <ul class="main-nav__category-menu">
                      <li><a class="main-nav__item" href="#">Your Account</a></li>
                      <li><a class="main-nav__item" href="#">Help</a></li>
                      <li><a class="main-nav__item" href="#">Sign Out</a></li>
                  </ul>
              </div>

          </div>
      </div>
      <label class="menu__full-bg-close" for="menu__toggle">
          <span></span>
      </label>
  </div>
</template>

<script>
    export default {
        name: 'Drawer',
        props: {
           
        },
        components: {
            
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >

</style>
