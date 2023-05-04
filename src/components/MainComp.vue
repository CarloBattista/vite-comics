<script>
export default {
    name: "MainComp",
}
</script>

<template>
    <!-- MainView -->
    <div class="mainView">
        <!-- Container Hero -->
        <div class="container__hero">
            <img class="hero_img" src="https://bleedingcool.com/wp-content/uploads/2020/06/DC-Comics-Spotify-Logo-1200x628.jpg" alt="hero image">
        </div>
        <!-- Container content -->
        <div class="container__content">
            <div class="inner_content">
                <div class="container_heading">
                    <h2 class="heading_content">Current Series</h2>
                </div>
                <div class="container_series"></div>
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