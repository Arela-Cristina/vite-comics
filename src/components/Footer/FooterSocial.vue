<!-- codice Javascript -->
<script>
export default {
    name: "FooterSocial",
}

</script>

<!-- Codice HTML -->
<template>
    <section>
        <span id="signUp">Sign Up Now</span>
        <div>
            <span>Follow Us</span>
            <img src="../../../public/img/footer-pinterest.png" alt="link pinterest">
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

div {
    display: flex;
    align-items: center;
    gap: 10px;
}

span {
    color:#0282f9;
    font-weight: bolder;
}

img {
    width: 25px;
}
</style>