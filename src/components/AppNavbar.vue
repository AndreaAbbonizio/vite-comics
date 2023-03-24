<script>
export default {
    data() {
        return {
            navbarLinks: [
                'characters', 'comics', 'movies', 'tv', 'games', 'collectibles', 'videos', 'fans', 'news', 'shop'
            ]
        }
    },
}
</script>


<template>
    <nav>
        <div class="container-image-navbar">
            <img src="/img/dc-logo.png" alt="Logo">
        </div>

        <div class="container-link-navbar">
            <ul>
                <li v-for="link in navbarLinks">{{ link }}</li>
            </ul>
        </div>
    </nav>
</template>


<style lang="scss" scoped>
nav {
    display: flex;
    justify-content: space-around;
    padding-top: 40px;
    height: 100px;
    margin-bottom: 1em;

    .container-image-navbar {
        height: 80px;

        img {
            height: 100%;
            transform: translateY(-20px);
        }
    }

    .container-link-navbar ul {
        display: flex;
        height: 100%;
        align-items: center;

        li {
            padding: 20px;
            padding-bottom: 40px;
            text-transform: uppercase;
        }

        li:hover {
            color: #0c7cec;
            border-bottom: 3px solid #0c7cec;
        }

    }
}
</style>
