<template>
    <div class = "a-card h-full flex flex-col items-center bg-[color:var(--clr-primary)] p-4">
        <img class = "w-full aspect-square" :src= elem.poster  alt= elem.title>
        <h2 class= "text-white font-bold text-xxl text-center" >{{elem.title}}</h2>
        <div class = "text-[color:var(--clr-tertiary)]">{{elem.author}}</div>
        <small class = "text-[color:var(--clr-tertiary)]">{{elem.year}}</small>
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

</style>