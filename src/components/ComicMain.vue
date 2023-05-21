<script>
</script>

<template>
    <div class="main_top">
        <img src="../assets/img/jumbotron.jpg" alt="jumbotron" class="jumbo">
        <button class="series">CURRENT SERIES</button>
    </div>
    <div class="main_bottom">
        <div class="container">
            <ul>
                <li>
                    <a href="#"><span>DIGITAL COMICS</span></a>
                </li>
                <li>
                    <a href="#"><span>DC MERCHANDISE</span></a>
                </li>
                <li>
                    <a href="#"><span>SUBSCRIPTION</span></a>
                </li>
                <li>
                    <a href="#"><span>COMIC SHOP LOCATOR</span></a>
                </li>
                <li>
                    <a href="#"><span>DC POWER VISA</span></a>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use './../assets/style/partials/container' as *;

.main_top {
    position: relative;

    .jumbo {
        display: block;
        height: 300px;
        width: 100%;
        object-fit: cover;
        object-position: top;
    }

    .series {
        background-color: #0282F9;
        color: white;
        font-size: 18px;
        padding: 0.5rem 1rem;
        border: 1px solid #0282F9;
        position: absolute;
        bottom: -20px;
        left: 300px
    }
}

.main_bottom {
    height: 500px;
    background-color: #1C1C1C;

    .container {
        @include container_general;

        ul {
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: space-around;
            gap: .5rem;
        }

    }


}
</style>
