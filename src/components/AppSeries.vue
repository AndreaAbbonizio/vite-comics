<script>
export default {
    data() {
        return {

        }
    },
    props: {
        img: String,
        title: String,
    }
}
</script>


<template>
    <div class="card-series">
        <img :src="img" alt="">
        <p id="title">{{ title }}</p>
    </div>
</template>


<style lang="scss" scoped>
.card-series {
    width: calc(100% / 6 - 20px * 5 / 6);
    padding-top: 40px;


    img {
        height: 135px;
        width: 100%;
        object-fit: fill;
    }

    #title {
        color: white;
        padding-top: .5em;
    }

}
</style>