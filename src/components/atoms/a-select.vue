<template>
  <form class = "flex flex-col gap-2">
      <label class = "text-white text-lg font-semibold" for="genre">Seleziona per genere</label>
      <select v-model = "sharedData.selectOption" class= "font-semibold rounded-md" name="genre" id="">
          <option value="">Tutti i generi</option>
          <option v-for = "(elem, index) in sharedData.typeOption"
          :key = "index"
          :value = "elem">
          {{elem}}
          </option>
      </select>
  </form>
</template>

<script>

import sharedData from '../../shared/sharedData.js'

export default {
    name: "genreSelect",
    data(){
        return {
            sharedData,
        }
    }
}
</script>

<style lang = "scss" scoped>

</style>