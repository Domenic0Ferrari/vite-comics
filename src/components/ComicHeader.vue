<script>
</script>

<template>
    <header>
        <div class="container">
            <div class="quadrato"></div>
            <ul>
                <li>
                    <a href="#">CIAO</a>
                </li>
                <li>
                    <a href="#">CIAO</a>
                </li>
                <li>
                    <a href="#">CIAO</a>
                </li>
                <li>
                    <a href="#">CIAO</a>
                </li>
                <li>
                    <a href="#">CIAO</a>
                </li>
                <li>
                    <a href="#">CIAO</a>
                </li>
                <li>
                    <a href="#">CIAO</a>
                </li>
                <li>
                    <a href="#">CIAO</a>
                </li>
                <li>
                    <a href="#">CIAO</a>
                </li>
                <li>
                    <a href="#">CIAO</a>
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
        list-style: none;
        gap: .7rem;

        a {
            text-decoration: none;
            color: #585350;

            &:hover {
                color: #0282F9;
            }
        }
    }
}
</style>
