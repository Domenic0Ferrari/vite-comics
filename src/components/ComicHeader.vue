<script>
export default {
    data() {
        return {
            vociMenu: [
                'CHARACTCERS',
                'COMICS',
                'MOVIE',
                'TV',
                'GAMES',
                'COLLECTIBLES',
                'VIDEO',
                'FANS',
                'NEWS',
                'SHOP']
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <img src="../assets/img/dc-logo.png" alt="#">
            <ul>
                <li v-for="voce in vociMenu">
                    <a href="#">{{ voce }}</a>
                </li>
            </ul>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use './../assets/style/general.scss' as *;
@use './../assets/style/partials/container' as *;

header {
    background-color: white;

    .container {
        @include container_general;
        background-color: #FFFF;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    ul {
        display: flex;
        gap: 1rem;

        a {
            color: #585350;

            &:hover {
                padding-bottom: 2rem;
                border-bottom: 5px solid #0282F9;
                color: #0282F9;
            }
        }
    }
}
</style>
