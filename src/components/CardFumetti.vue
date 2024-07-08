<script>

export default {
    name: "CardFumetti",
    props: {
        details: Object
    }
}
</script>

<template>
    <div class="box-fumeto">
        <img :src="details.thumb" alt="comic">
        <span class="caption">{{details.series}}</span>
    </div>
</template>

<style scoped>
pre {
    color: white;
}

.box-fumeto {
    width: calc(100% / 6 - 2rem);
}

img {
    width: 100%;
    height: 80%;
   
}

.caption {
    color: white;
    font-size: 12px;
}
</style>