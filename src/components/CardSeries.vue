<script>

export default {
    name: "CardSeries",
    props: ["cardInfo"]
}

</script>

<template>
    <div class="cardSeries">
        <a href="/">
            <div class="imgWrap">
                <img class="img_series" :src="cardInfo.thumb" :alt="'image of ' + cardInfo.series">
            </div>
            <div class="infoWrap">
                <p class="title_series">{{ cardInfo.series }}</p>
            </div>
        </a>
    </div>
</template>

<style lang="scss" scoped></style>