<!-- codice Javascript -->
<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "Characters",
                    url: "#",
                    current: false,
                },
                {
                    text: "Comics",
                    url: "#",
                    current: false,
                },
                {
                    text: "Movies",
                    url: "#",
                    current: false,
                },
                {
                    text: "TV",
                    url: "#",
                    current: false,
                },
                {
                    text: "Games",
                    url: "#",
                    current: false,
                },
                {
                    text: "Collectibles",
                    url: "#",
                    current: false,
                },
                {
                    text: "Videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "Fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "News",
                    url: "#",
                    current: false,
                },
                {
                    text: "Shop",
                    url: "#",
                    current: false,
                }
            ]
        }
    }
}


</script>

<!-- Codice HTML -->
<template>
    <!-- logo -->
    <div>
        <img src="/public/img/dc-logo.png">

        <!-- menu header -->
        <ul>
            <li v-for="(link, index) in links" :key="index"><a href="#">{{ link.text }}</a></li>
        </ul>
    </div>
</template>

<!-- Codice Css -->
<style scoped>
div {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-left: 10rem;
    padding-right: 10rem;
    padding-top: 1rem;
    padding-bottom: 1rem;
    /* debug */
    background-color: pink;
}

img {
    width: 50px;
}

ul {
    display: flex;
    gap: 1rem;
    list-style: none;
}

a {
    text-decoration: none;
}
</style>