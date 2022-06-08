<template>
  <form class = "flex flex-col gap-2">
      <label class = "text-white text-lg font-semibold" for="genre">Seleziona per genere</label>
      <select v-model = "sharedData.selectOption" class= "font-semibold rounded-md" name="genre" id="">
          <option value="">Tutti i generi</option>
          <option value="Rock">Rock</option>
          <option value="Pop">Pop</option>
          <option value="Jazz">Jazz</option>
          <option value="Metal">Metal</option>
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