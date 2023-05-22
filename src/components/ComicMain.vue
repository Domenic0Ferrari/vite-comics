<script>
import cardMain from './cardMain.vue';
export default {
    data() {
        return {
            arrComics: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    },
    components: {

        cardMain,
    }
}
</script>

<template>
    <div class="main_top">
        <img src="../assets/img/jumbotron.jpg" alt="jumbotron" class="jumbo">
        <button class="series">
            <a href="#">CURRENT SERIES</a>
        </button>
    </div>
    <div class="main_center">
        <div class="container">
            <ul>
                <li>
                    <cardMain v-for="comic in arrComics" :key="comic.series" :thumb="comic.thumb" :series="comic.series" />
                </li>
            </ul>
            <button class="more">
                <a href="#">LOAD MORE</a>
            </button>
        </div>
    </div>
    <div class="main_bottom">
        <div class="container">
            <div class="square">
                <div class="img_square">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="#">
                </div>
                <a href="#">DIGITAL COMICS</a>
            </div>
            <div class="square">
                <div class="img_square">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="#">
                </div>
                <a href="#">DC MERCHANDISE</a>
            </div>
            <div class="square">
                <div class="img_square">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="#">
                </div>
                <a href="#">SUBSCRIPTION</a>
            </div>
            <div class="square">
                <div class="img_square">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="#">
                </div>
                <a href="#">COMIC SHOP LOCATOR</a>
            </div>
            <div class="square">
                <div class="img_square">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="#">
                </div>
                <a href="#">DC POWER VISA</a>
            </div>
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
        font-size: 18px;
        padding: 0.5rem 1rem;
        border: 1px solid #0282F9;
        position: absolute;
        bottom: -20px;
        left: 300px;

        a {
            color: white;
        }
    }
}

.main_center {
    background-color: #1C1C1C;

    .container {
        @include container_general;
        padding: 2rem 0;

        li {
            display: flex;
            flex-wrap: wrap;
            gap: .5rem;
            justify-content: space-between;
        }
    }

    .more {
        background-color: #0282F9;
        font-size: 18px;
        padding: 0.5rem 1rem;
        border: 1px solid #0282F9;

        a {
            color: white;
        }
    }
}

.main_bottom {
    background-color: #0282F9;

    .container {
        @include container_general;
        display: flex;
        justify-content: space-around;
        align-items: center;

        .square {
            height: 150px;
            display: flex;
            align-items: center;
            gap: 1rem;

            .img_square {
                height: 50px;
                width: 45px;

                img {
                    height: 100%;
                    width: 100%;
                }
            }

            a {
                font-size: 14px;
                color: white;
            }
        }

    }
}
</style>
