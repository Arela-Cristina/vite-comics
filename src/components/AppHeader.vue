<!-- codice Javascript -->
<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                { // 0
                    text: "Characters",
                    url: "#",
                },
                { // 1
                    text: "Comics",
                    url: "#",
                },
                { // ...
                    text: "Movies",
                    url: "#",
                },
                {
                    text: "TV",
                    url: "#",
                },
                {
                    text: "Games",
                    url: "#",
                },
                {
                    text: "Collectibles",
                    url: "#",
                },
                {
                    text: "Videos",
                    url: "#",
                },
                {
                    text: "Fans",
                    url: "#",
                },
                {
                    text: "News",
                    url: "#",
                },
                {
                    text: "Shop",
                    url: "#",
                }
            ],
            current: undefined
        }
    },
    methods:{
        setCurrent(link){
            this.current = link;
        }
    },
    mounted() {
        this.current = this.links[0];
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
            <li v-for="(link, index) in links" :key="index"><a href="#" @click="setCurrent(link)" :class="link == current ? 'active' : ''">{{ link.text }}</a>
            </li>
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
    background-color: white;
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

.active {
    border-bottom: solid 4px #2196F3;
    padding-bottom: 28px;
    color: #2196F3;
}

a:hover {
    border-bottom: solid 4px #2196F3;
    padding-bottom: 28px;
    color: #2196F3;
}
</style>