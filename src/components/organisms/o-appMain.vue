<template>
  <main class="flex justify-center items-center">
      <appContent/>
  </main>
</template>

<script>

import appContent from "./o-appContent.vue"

export default {
    name: "appMain",
    components: {
        appContent,
    }
}
</script>

<style lang = "scss" scoped>
    main{
        min-height: calc(100vh - var(--header-height));
        background-color: var(--clr-bg-secondary);
    }
</style>