<template>
  <div id="app">
    <appHeader/>
    <mainHeader/>
  </div>
</template>

<script>

import appHeader from './components/organisms/o-appHeader.vue';
import mainHeader from './components/organisms/o-appMain.vue';

export default {
  name: 'App',
  components: {
    appHeader,
    mainHeader,
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';


</style>
