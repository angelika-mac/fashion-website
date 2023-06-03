<template>
    <div id="main-componenet-wrapper">
        <nav-bar-component></nav-bar-component>
        <hero-component></hero-component>
        <deals-component></deals-component>
    </div>
</template>

<script>
import NavBarComponent from './NavBarComponent.vue'
import HeroComponent from './HeroComponent.vue';
import DealsComponent from './DealsComponent.vue';
export default {
  components: { NavBarComponent, HeroComponent, DealsComponent },

}
</script>

<style>

</style>