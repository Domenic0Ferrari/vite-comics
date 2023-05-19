<script>
</script>

<template>
    <div class="container">
        <div class="main_top">
            <span class="content"> CONTENT GOES HERE </span>
        </div>
        <div class="main_bottom">
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

.container {
    @include container_general;

    .main_top {
        height: 100px;
        background-color: #1C1C1C;

        .content {
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
    }

    .main_bottom {
        height: 100px;
        background-color: #0282F9;

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
