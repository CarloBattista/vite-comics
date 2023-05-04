<script>
import CardSeries from "./CardSeries.vue"

export default {
    name: "MainComp",
    components: {
        CardSeries,
    },
    data() {
        return {
            series: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel",
                },
            ]
        }
    }
}
</script>

<template>
    <!-- MainView -->
    <div class="mainView">
        <!-- Container Hero -->
        <div class="container__hero">
            <img class="hero_img"
                src="https://bleedingcool.com/wp-content/uploads/2020/06/DC-Comics-Spotify-Logo-1200x628.jpg"
                alt="hero image">
        </div>
        <!-- Container content -->
        <div class="container__content">
            <div class="inner_content">
                <div class="container_heading">
                    <h2 class="heading_content">Current Series</h2>
                </div>
                <div class="container_series">
                    <CardSeries v-for="(element, index) in series"/>
                    <!-- <div class="cardSeries" v-for="(element, index) in series" :key="index">
                        <a href="/">
                            <div class="imgWrap">
                                <img class="img_series" :src="element.thumb" :alt="'image of ' + element.series">
                            </div>
                            <div class="infoWrap">
                                <p class="title_series">{{ element.series }}</p>
                            </div>
                        </a>
                    </div> -->
                </div>
            </div>
        </div>
        <!-- Container Banner -->
        <div class="container__banner">
            <div class="inner_content">
                <!-- Container Card -->
                <div class="row_container">
                    <!-- Card -->
                    <div class="row_card">
                        <a href="/digital-comics">
                            <img class="imgText" src="/imgs/buy-comics-digital-comics.png" alt="">
                            <span class="cardText">Digital Comics</span>
                        </a>
                    </div>
                    <div class="row_card">
                        <a href="/dc-merchandise">
                            <img class="imgText" src="/imgs/buy-comics-merchandise.png" alt="">
                            <span class="cardText">Dc Merchandise</span>
                        </a>
                    </div>
                    <div class="row_card">
                        <a href="/subscription">
                            <img class="imgText" src="/imgs/buy-comics-subscriptions.png" alt="">
                            <span class="cardText">Subscription</span>
                        </a>
                    </div>
                    <div class="row_card">
                        <a href="/comic-shop-location">
                            <img class="imgText" src="/imgs/buy-comics-shop-locator.png" alt="">
                            <span class="cardText">Comic Shop Location</span>
                        </a>
                    </div>
                    <div class="row_card">
                        <a href="/dc-power-visa">
                            <img class="imgText" src="/imgs/buy-dc-power-visa.svg" alt="">
                            <span class="cardText">Dc Power Visa</span>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>