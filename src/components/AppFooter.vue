<script>
export default {
    data() {
        return {
            footerLinks: [
                {
                    title: 'DC Comics',
                    links: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News'],
                },
                {
                    title: 'Shop',
                    links: ['Shop Dc', 'Shop Dc Collectibles'],
                },
                {
                    title: 'Dc',
                    links: ['Terms Of Use', 'Privacy Policy(New)', 'Ad Choisese', 'Advertising', 'Jobs', 'Subscriptions', 'Talent WorkShops', 'CSPSC Certificates', 'Rating', 'Shop Help', 'Contact Us'],
                },
                {
                    title: 'Sites',
                    links: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa'],
                },
            ]
        }
    },
}
</script>

<template>
    <div id="container-footer">
        <div id="container-list">
            <ul v-for="element in footerLinks">
                <h2>{{ element.title }}</h2>
                <li v-for="link in element.links">{{ link }}</li>
            </ul>

            <div id='background-logo'>
                <img src="/img/dc-logo-bg.png" alt="">
            </div>
        </div>

    </div>
</template>


<style lang="scss" scoped>
#container-footer {
    position: relative;
    background-image: url("/img/jumbotron.jpg");
    background-size: cover;

    #container-list {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        align-content: flex-start;
        height: 350px;
        max-width: 1200px;
        margin: 0 auto;
        padding: 20px;
    }

    h2 {
        color: white;
        z-index: 2;
    }

    ul {
        width: 200px;
        z-index: 2;
        color: darkgrey;

    }

    &::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: black;
        opacity: 0.8;

    }

    #background-logo {
        z-index: 2;
        width: 500px;
        height: 500px;
        transform: translateY(-25%);

        img {
            height: 100%;
        }

    }

}
</style>
