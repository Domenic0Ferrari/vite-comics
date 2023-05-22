<script>
</script>

<template>
    <footer>
        <div class="footer_top">
            <div class="container">
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
                <div class="footer_img">
                    <img src="../assets/img/dc-logo-bg.png" alt="#">
                </div>
            </div>
        </div>
        <div class="footer_bottom">
            <div class="container">
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




.footer_top {
    height: 300px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    padding-top: 1rem;

    .container {
        @include container_general;
        display: flex;
        gap: 1.5rem;

        .column {
            display: flex;
            flex-direction: column;
            gap: .2rem;

            a {
                color: gainsboro;
                font-size: 10px;
            }
        }

        .footer_img {
            height: 450px;
            position: absolute;

            img {
                height: 100%;
                position: relative;
                top: -100px;
                left: 550px;
            }
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
