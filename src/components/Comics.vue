<template>
    <div class="comics-series">
        <img :src="ComicObject.thumb" :alt="ComicObject.series">
        <h4>{{ ComicObject.series }}</h4>
    </div>
</template>

<script>
export default {
    name: 'Comics',
    props: ['ComicObject']
}
</script>

<style scoped leng="scss">

.comics-series {
    width: calc( (100% / 6) - 20px );
    margin: 10px;
    padding-bottom: 20px;
    color: white;
}

</style>