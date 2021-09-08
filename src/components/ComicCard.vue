<template>
    <div class="comic_card">
        <div class="square" :style="{ 'background-image': 'url(' + comic.thumb + ')' }">
        </div>
        <h5>{{comic.series}}</h5>
    </div>
</template>

<script>
export default {
name: 'ComicCard', 
props: ['comic'],
}
</script>

<style lang="scss" scoped>
.comic_card {
    flex-basis: calc(100% / 6);
    padding: 15px;

    h5 {
        margin-top: 10px;
    }

    .square {
        width: 100%;
        background-position: top;
        background-size: cover;
    }

    .square:after {
        content: "";
        display: block;
        padding-bottom: 100%;
    }
}
</style>