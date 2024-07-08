<!-- codice Javascript -->
<script>
export default {
    name: "FooterStore",
}

</script>

<!-- Codice HTML -->
<template>
    <section>
        <!-- contenuto dinamico -->
        <div>
            <img src="../../../public/img/buy-comics-digital-comics.png" alt="">
            <a href="#">Digital Comics</a>
        </div>
        <!-- contenuto da cancellare quando si isneria il conetnuto dinamico -->
        <div>
            <img src="../../../public/img/buy-comics-digital-comics.png" alt="">
            <a href="#">Digital Comics</a>
        </div>
        <div>
            <img src="../../../public/img/buy-comics-digital-comics.png" alt="">
            <a href="#">Digital Comics</a>
        </div>
        <div>
            <img src="../../../public/img/buy-comics-digital-comics.png" alt="">
            <a href="#">Digital Comics</a>
        </div>
        <div>
            <img src="../../../public/img/buy-comics-digital-comics.png" alt="">
            <a href="#">Digital Comics</a>
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
    width: 2.5rem;
}
</style>