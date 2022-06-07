<template>
  <main class="min-h-[calc(100vh-var(--header-height))] flex justify-center items-center bg-[color:var(--clr-bg-secondary)]">
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

</style>