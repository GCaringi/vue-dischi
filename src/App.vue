<template>
  <div id="app">
    <appLoader/>
    <appHeader/>
    <mainHeader/>
  </div>
</template>

<script>

import appLoader from './components/organisms/o.appLoader.vue'
import appHeader from './components/organisms/o-appHeader.vue';
import mainHeader from './components/organisms/o-appMain.vue';

export default {
  name: 'App',
  components: {
    appHeader,
    mainHeader,
    appLoader,
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';

#app{
  position: relative;
}
</style>
