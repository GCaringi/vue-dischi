<template>
    <div>
        <img :src= elem.poster  alt="IMG">
        <h2>Titolo</h2>
        <div>Artista</div>
        <small>Year</small>
    </div>
</template>

<script>
export default {
    name: "playlistCard",
    props: {
        elem: {
            type: Object,
            required: true,
        }
    }
}
</script>

<style lang = "scss" scoped>

img{
    width: 50%;
}

</style>