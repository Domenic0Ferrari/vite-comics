<script>
</script>

<template>
    <footer>
        <div class="container">
            <div class="footer_top"></div>
            <div class="footer_bottom"></div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use './../assets/style/partials/container' as *;

.container {
    @include container_general;
}


.footer_top {
    height: 250px;
    background-color: bisque;
}

.footer_bottom {
    height: 150px;
    background-color: #303030;
}
</style>
