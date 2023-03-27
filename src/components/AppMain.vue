<script>
export default {
    data() {
        return {
            mainLinks: [
                {
                    title: 'Digital Comics',
                    image: '/img/buy-comics-digital-comics.png',
                },
                {
                    title: 'Dc Merchandise',
                    image: '/img/buy-comics-merchandise.png',
                },
                {
                    title: 'Subscription',
                    image: '/img/buy-comics-subscriptions.png',
                },
                {
                    title: 'Comic Shop Location',
                    image: '/img/buy-comics-shop-locator.png',
                },
                {
                    title: 'Dc Power Visa',
                    image: '/img/buy-dc-power-visa.svg',
                }
            ],
        }
    },
}
</script>

<template>
    <div id="container-main">
        <div id="main-links">
            <ul>
                <li v-for="link in mainLinks">
                    <img :src='link.image' alt="">
                    <span>{{ link.title }}</span>
                </li>
            </ul>
        </div>
    </div>
</template>


<style lang="scss" scoped>
#container-main {
    position: relative;
    z-index: 3;
    background-color: #0c7cec;
    color: white;


    #main-links {
        max-width: 1000px;
        margin: 0 auto;
        height: 200px;


        ul {
            display: flex;
            align-items: center;
            justify-content: space-between;

            height: 100%;

            li {
                display: flex;
                align-items: center;

                height: 50px;
                gap: .5em;
                text-transform: uppercase;

                img {
                    height: 100%;
                }

                span {
                    font-size: .8em;
                }
            }


        }



    }
}
</style>
