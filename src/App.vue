<template>
  <div id="app">
    <AppHeader/>
    <AppMain/>
    <AppPreFooter/>
    <AppFooter/>
    
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppPreFooter from './components/AppPreFooter.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppPreFooter,
    AppFooter,
},
};
</script>

<style lang="scss">
@import "./style/common.scss"


</style>
