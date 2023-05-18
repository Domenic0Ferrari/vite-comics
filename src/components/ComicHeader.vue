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

header {
    background-color: white;

    .container {
        max-width: 1000px;
        padding-inline: 0.2rem;
        background-color: salmon;
        margin-inline: auto;
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
