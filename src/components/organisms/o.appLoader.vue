<template>
  <div class="loader">
      <loaderItem/>
  </div>
</template>

<script>

import loaderItem from '../atoms/a-loader.vue'

export default {
    name: "appLoader",
    components: {
        loaderItem,
    }
}
</script>

<style>
    .loader{
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        inset: 0;
        background-color: rgba(255, 0, 0, 0.138) ;
    }
</style>