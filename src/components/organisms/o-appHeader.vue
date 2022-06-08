<template>
  <header class = "bg-[color:var(--clr-primary)] h-[var(--header-height)] flex items-center justify-between px-3">
      <logo/>
      <genre-select/>
  </header>
</template>

<script>

import logo from '../atoms/a-logo.vue';
import genreSelect from '../atoms/a-select.vue';

export default {
    name : "appHeader",
    components : {
        logo,
        genreSelect,
    }
}
</script>

<style lang = "scss" scoped>


</style>