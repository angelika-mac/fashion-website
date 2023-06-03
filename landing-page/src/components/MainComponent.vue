<template>
    <div id="main-componenet-wrapper">
        <nav-bar-component></nav-bar-component>
        <hero-component></hero-component>
        <deals-component></deals-component>
        <trending-component></trending-component>
        <new-product-component></new-product-component>
        <recents-component-vue></recents-component-vue>
        <inspo-component></inspo-component>
        <footer-component></footer-component>
    </div>
</template>

<script>
import NavBarComponent from './NavBarComponent.vue'
import HeroComponent from './HeroComponent.vue';
import DealsComponent from './DealsComponent.vue';
import TrendingComponent from './TrendingComponent.vue';
import NewProductComponent from './NewProductComponent.vue';
import RecentsComponentVue from './RecentsComponent.vue';
import InspoComponent from './InspoComponent.vue';
import FooterComponent from './FooterComponent.vue';
export default {
  components: { NavBarComponent, HeroComponent, DealsComponent , TrendingComponent, NewProductComponent, RecentsComponentVue, InspoComponent, FooterComponent},

}
</script>