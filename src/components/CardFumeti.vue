<!-- codice Javascript -->
<script>
export default {
    name: "CardFumeti",
    props: {
        details: Object,
    }
}

</script>

<!-- Codice HTML -->
<template>
    <section>
        <div class="box-fumetto">
            <img :src="details.thumb" alt="comic">
            <div class="caption">{{details.type}}</div>
        </div>
    </section>
</template>

<!-- Codice Css -->
<style scoped>
section {
    background-color: rgb(24, 24, 24);
    width: 100%;
    min-height: 10rem;
    padding-left: 10rem;
    padding-right: 10rem;
    padding-top: 3rem;
    padding-bottom: 3rem;
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;

}

.box-fumetto {
    width: calc(100% / 6 - 1rem);
}

img {
    width: 100%;
}

.caption {
    color: white;
    font-size: 12px;
}
</style>