<!-- codice Javascript -->
<script>
export default {
    name: "FooterSocial",
    data() {
        return {
            arraySocial: [
                {
                    logo: "./public/img/footer-facebook.png",
                    url: "#",
                    current: false,
                },
                {
                    logo: "./public/img/footer-twitter.png",
                    url: "#",
                    current: false,
                },
                {
                    logo: "./public/img/footer-youtube.png",
                    url: "#",
                    current: false,
                },
                {
                    logo: "./public/img/footer-pinterest.png",
                    url: "#",
                    current: false,
                },
                {
                    logo: "./public/img/footer-periscope.png",
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
    <section>
        <span id="signUp">Sign Up Now</span>
        <div class="box-social">

            <span>Follow Us</span>
            <div v-for="(social, index) in arraySocial" :key="index">
                <img :src="social.logo" alt="">
            </div>
        </div>
    </section>
</template>

<!-- Codice Css -->
<style scoped>
section {
    background-color: rgb(37, 36, 36);
    height: 4.5rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-left: 10rem;
    padding-right: 10rem;
}

#signUp {
    border: 2px solid #0282f9;
    padding: 8px 8px;
    color: white;
    font-weight: bolder;
}

div.box-social {
    display: flex;
    align-items: center;
    gap: 10px;
}

span {
    color: #0282f9;
    font-weight: bolder;
}

img {
    width: 25px;
}
</style>