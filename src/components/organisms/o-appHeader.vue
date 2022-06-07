<template>
  <header>
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

header{
    background-color: var(--clr-primary);
    height: var(--header-height);
}

</style>