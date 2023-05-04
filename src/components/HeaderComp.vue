<script>
export default {
    name: "HeaderComp",
    data() {
        return {
            menuVisible: false,
            isOpen: false,
        }
    },
    computed: {
        isOpen() {
            return this.menuVisible ? 'fa-solid fa-xmark' : 'fa-solid fa-bars';
        }
    },
    methods: {
        triggerMenuMobile() {
            if (this.menuVisible == false) {
                this.menuVisible = true;
            } else {
                this.menuVisible = false;
            }
        }
    },
}
</script>

<template>
    <!-- Header -->
    <div class="header">
        <div class="inner_header">
            <!-- Logo -->
            <a href="/" class="logoSite">
                <img class="icon_logo" src="/imgs/dc-logo.png" alt="">
            </a>
            <!-- Nav -->
            <ul class="nav">
                <li class="listItem">
                    <a class="linkPage" href="/characters">Characters</a>
                </li>
                <li class="listItem currentPage">
                    <a class="linkPage" href="/comics">Comics</a>
                </li>
                <li class="listItem">
                    <a class="linkPage" href="/movies">Movies</a>
                </li>
                <li class="listItem">
                    <a class="linkPage" href="/tv">Tv</a>
                </li>
                <li class="listItem">
                    <a class="linkPage" href="/games">Games</a>
                </li>
                <li class="listItem">
                    <a class="linkPage" href="/collectibles">Collectibles</a>
                </li>
                <li class="listItem">
                    <a class="linkPage" href="/videos">Videos</a>
                </li>
                <li class="listItem">
                    <a class="linkPage" href="/fans">Fans</a>
                </li>
                <li class="listItem">
                    <a class="linkPage" href="/news">News</a>
                </li>
                <li class="listItem">
                    <a class="linkPage" href="/shop">Shop</a>
                </li>
            </ul>
            <!-- Mobile -->
            <div class="box_func_hamburger">
                <!-- Button hamburger trigger -->
                <button class="btn_trigger_hamburger" @click="triggerMenuMobile">
                    <i class="" :class="isOpen"></i>
                </button>
                <!-- Hamburger menu -->
                <div class="hamburger_menu" v-show="menuVisible">
                    <ul class="list_nav_mobile">
                        <li class="list_mobile">
                            <a class="linkPage" href="/characters">Characters</a>
                        </li>
                        <li class="list_mobile">
                            <a class="linkPage mobile_page_active" href="/comics">Comics</a>
                        </li>
                        <li class="list_mobile">
                            <a class="linkPage" href="/movies">Movies</a>
                        </li>
                        <li class="list_mobile">
                            <a class="linkPage" href="/tv">Tv</a>
                        </li>
                        <li class="list_mobile">
                            <a class="linkPage" href="/games">Games</a>
                        </li>
                        <li class="list_mobile">
                            <a class="linkPage" href="/collectibles">Collectibles</a>
                        </li>
                        <li class="list_mobile">
                            <a class="linkPage" href="/videos">Videos</a>
                        </li>
                        <li class="list_mobile">
                            <a class="linkPage" href="/fans">Fans</a>
                        </li>
                        <li class="list_mobile">
                            <a class="linkPage" href="/news">News</a>
                        </li>
                        <li class="list_mobile">
                            <a class="linkPage" href="/shop">Shop</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<style></style>