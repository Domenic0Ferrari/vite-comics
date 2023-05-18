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
header {
    background-color: white;

    .container {
        max-width: 1000px;
        height: 100px;
        background-color: salmon;
        margin-inline: auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .quadrato {
        height: 100%;
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
                color: blue;
            }
        }
    }
}
</style>
