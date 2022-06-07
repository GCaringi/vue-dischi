<template>
  <div class="loader flex justify-center items-center absolute inset-0 bg-[color:var(--clr-bg-secondary)]"
        v-if = !isLoad>
      <loaderItem/>
  </div>
</template>

<script>

import loaderItem from '../atoms/a-loader.vue'

export default {
    name: "appLoader",
    data(){
        return {
            isLoad: false,
        }
    },
    mounted(){
        document.onreadystatechange = () => {
            if (document.readyState == "complete"){
                this.isLoad = true;
            }
        }
    },
    components: {
        loaderItem,
    }
}
</script>

<style lang = "scss" scoped>

</style>