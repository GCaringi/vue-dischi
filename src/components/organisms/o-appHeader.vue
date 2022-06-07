<template>
  <header class = "bg-[color:var(--clr-primary)] h-[var(--header-height)]">
      <logo/>
  </header>
</template>

<script>

import logo from '../atoms/a-logo.vue'

export default {
    name : "appHeader",
    components : {
        logo
    }
}
</script>

<style lang = "scss" scoped>


</style>