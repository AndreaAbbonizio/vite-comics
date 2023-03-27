<script>
export default {
    data() {
        return {

        }
    },
}
</script>

<template>
    <div id="container-bg-footer-nav">
        <div id="container-footer-nav">
            <button>
                SIGN-UP NOW
            </button>
            <div id="container-icons">
                <span><strong> FOLLOW US </strong></span>
                <img src="/img/footer-facebook.png" alt="">
                <img src="/img/footer-periscope.png" alt="">
                <img src="/img/footer-pinterest.png" alt="">
                <img src="/img/footer-twitter.png" alt="">
                <img src="/img/footer-youtube.png" alt="">

            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
#container-bg-footer-nav {
    position: relative;
    background-color: #303030;
    padding: 20px;

    #container-footer-nav {
        display: flex;
        justify-content: space-between;
        max-width: 1000px;
        margin: 0 auto;


        button {
            padding: 10px;
            color: white;
            border-color: #0c7cec;
            background-color: #303030;
        }

    }

    #container-icons {
        display: flex;
        align-items: center;
        gap: 10px;


        strong {
            color: #0c7cec;
        }
    }

}
</style>


