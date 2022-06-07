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
        height: 100%;
        background-color: var(--clr-bg-secondary);
    }
</style>