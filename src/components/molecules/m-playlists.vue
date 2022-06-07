<template>
    <div class="container grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-5 place-items-center py-5 gap-3">
        <card
        v-for = "(element, index) in myData"
        :key = "index"
        :elem = "element"
        />
    </div>
</template>

<script>

import card from '../atoms/a-card.vue';
import axios from 'axios';

export default {
    name: "playLists",
    data(){
        return {
            myData: [],
        }
    },
    components: {
        card,
    },
    created(){
        axios.get("https://flynn.boolean.careers/exercises/api/array/music")
        .then((apiData) =>{
            console.log(apiData.data.response)
            this.myData = apiData.data.response;
        })
        .catch(function(error){
            console.log(error)
        })

    }
}
</script>

<style lang = "scss" scoped>

</style>