<script>
export default {
    props: {
        thumb: String,
        series: String,

    }
};
</script>

<template>
    <div class="card">
        <img :src="thumb" :alt="series" class="img_card">
        <a href="#">{{ series }}</a>
    </div>
</template>

<style lang="scss" scoped>
.card {
    width: calc((100% / 6) - .5rem);

    .img_card {
        width: 100%;
        height: 200px;
    }

    a {
        color: white;
    }
}
</style>
