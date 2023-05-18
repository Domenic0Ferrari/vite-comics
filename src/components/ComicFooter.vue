<script>
</script>

<template>
    <footer>
        <div class="container">
            <div class="footer_top">
                <div class="column">
                    <span>DC COMICS
                    </span>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                </div>
                <div class="column">
                    <span>DC COMICS
                    </span>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                </div>
                <div class="column">
                    <span>DC COMICS
                    </span>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                    <a href="#">CIAO</a>
                </div>
            </div>
            <div class="footer_bottom">
                <button class="sign">SIGN-UP NOW!</button>
                <ul>
                    <li> <a href="#">FOLLOW US</a>
                    </li>
                    <li> <a href="#">CIAO</a>
                    </li>
                    <li> <a href="#">CIAO</a>
                    </li>
                    <li> <a href="#">CIAO</a>
                    </li>
                    <li> <a href="#">CIAO</a>
                    </li>
                    <li> <a href="#">CIAO</a>
                    </li>
                </ul>
            </div>
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
    background-color: orange;
    display: flex;
    gap: 1rem;
    padding-top: 1rem;

    .column {
        display: flex;
        flex-direction: column;
        gap: .2rem;

        a {
            color: #303030;
            font-size: 12px;
        }
    }
}

.footer_bottom {
    height: 150px;
    background-color: #303030;
    display: flex;
    justify-content: space-around;
    align-items: center;

    .sign {
        border: 2px solid blue;
        background-color: #303030;
        padding: 1rem;
    }

    ul {
        display: flex;
        gap: .5rem;

        a {
            color: white;
        }
    }
}
</style>
