<template>
    <div class = "a-card">
        <img :src= elem.poster  alt="IMG">
        <h2>{{elem.title}}</h2>
        <div>{{elem.author}}</div>
        <small>{{elem.year}}</small>
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
    width: 100%;
    aspect-ratio: 1;
}

.a-card{
    display: flex;
    flex-direction: column ;
    align-items: center;
    background-color: var(--clr-primary);
    padding: 20px;
}

</style>