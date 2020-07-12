<template>
 <header class="header">
    <SecondaryNavigation></SecondaryNavigation>
    <div id="main-header" class="main-header header__inner container-full container_inline">
        <div class="row container-full__row">
            <Drawer/>
            <a href="/" class="logo main-header__logo">
                <div class="logo__text"><span>Gam</span>body</div>
            </a>
            <PremiumOrStock/>
            <Search/>
            <Cart/>
        </div>
    </div>
    <div class="sticky-top"></div>
</header>
</template>

<script>
    import SecondaryNavigation from '../components/HeaderNavigation/SecondaryNavigation'
    import Drawer from '../components/HeaderNavigation/Drawer'
    import PremiumOrStock from '../components/HeaderNavigation/PremiumorStock'
    import Search from '../components/HeaderNavigation/Search'
    import Cart from '../components/HeaderNavigation/Cart'
    export default {
        name: 'Header',
        props: {
            msg: String
        },
        components: {
            SecondaryNavigation,
            Drawer,
            PremiumOrStock,
            Search,
            Cart
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >

</style>
