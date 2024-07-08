<!-- codice Javascript -->
<script>
export default {
    name: "FooterStore",
    data() {
        return {
            arrayItem: [
                {
                    src: "./public/img/buy-comics-digital-comics.png",
                    url: "#",
                    text: "Digital Comics",
                    current: false,
                },
                {
                    src: "./public/img/buy-comics-merchandise.png",
                    url: "#",
                    text: "DC Merchandise",
                    current: false,
                },
                {
                    src: "./public/img/buy-comics-subscriptions.png",
                    url: "#",
                    text: "Subscription",
                    current: false,
                },
                {
                    src: "./public/img/buy-comics-shop-locator.png",
                    url: "#",
                    text: "Comic Shop Locator",
                    current: false,
                },
                {
                    src: "./public/img/buy-dc-power-visa.svg",
                    url: "#",
                    text: "DC Power Visa",
                    current: false,
                }
            ]
        }
    }
}

</script>

<!-- Codice HTML -->
<template>
    <section>
        <!-- contenuto dinamico -->
        <div v-for="(item, index) in arrayItem" :key="index">
            <img :src="item.src" alt="">
            <a href="#">{{ item.text }}</a>
        </div>
    </section>
</template>

<!-- Codice Css -->
<style scoped>
section {
    display: flex;
    justify-content: space-between;
    padding-left: 11rem;
    padding-right: 11rem;
    width: 100%;
    height: 7rem;
    background-color: #0282f9;
}

div {
    display: flex;
    align-items: center;
    gap: 1rem;
}

img {
    width: 2.6rem;
    height: 3rem;
}
</style>