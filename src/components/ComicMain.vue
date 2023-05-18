<script>
</script>

<template>
    <div class="container">
        <div class="main_top"></div>
        <div class="main_bottom"></div>
    </div>
</template>

<style lang="scss" scoped>
@use './../assets/style/partials/container' as *;

.container {
    @include container_general;

    .main_top {
        height: 100px;
        background-color: #1C1C1C;
    }

    .main_bottom {
        height: 100px;
        background-color: #0282F9;
    }
}
</style>
