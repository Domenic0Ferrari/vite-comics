<script>
</script>

<template>
    <header>
        <div class="container">
            <div class="quadrato"></div>
            <ul>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">COMICS</a>
                </li>
                <li>
                    <a href="#">MOVIES</a>
                </li>
                <li>
                    <a href="#">TV</a>
                </li>
                <li>
                    <a href="#">GAMES</a>
                </li>
                <li>
                    <a href="#">COLLECTIBLES</a>
                </li>
                <li>
                    <a href="#">VIDEOS</a>
                </li>
                <li>
                    <a href="#">FANS</a>
                </li>
                <li>
                    <a href="#">NEWS</a>
                </li>
                <li>
                    <a href="#">SHOP</a>
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

    .quadrato {
        height: 100px;
        width: 100px;
        background-color: gold;
    }

    ul {
        display: flex;
        gap: .7rem;

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
