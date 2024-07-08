<!-- codice Javascript -->
<script>
export default {
    name: "FooterLinks",
}

</script>

<!-- Codice HTML -->
<template>
    <section>
        <!-- prima elenco di links -->
        <div class="mainBox">
            <div class="box">
                <div>
                    <span>DC COMICS</span>
                    <ul>
                        <li><a href="#">Characters</a></li>
                    </ul>
                </div>
                <!-- scondo elenco di links -->
                <div>
                    <span>SHOP</span>
                    <ul>
                        <li><a href="#">Characters</a></li>
                    </ul>
                </div>
            </div>
            <!-- terzo elenco di links -->
            <div>
                <span>DC</span>
                <ul>
                    <li><a href="#">Characters</a></li>
                </ul>
            </div>
            <!-- cuarto elenco di links -->
            <div>
                <span>SITES</span>
                <ul>
                    <li><a href="#">Characters</a></li>
                </ul>
            </div>
        </div>


        <img src="../../../public/img/dc-logo-bg.png" alt="dc logo">
    </section>
</template>

<!-- Codice Css -->
<style scoped>
section {
    position: relative;
    width: 100%;
    height: 20rem;
    background-image: url(../../../public/img/footer-bg.jpg);
}

.mainBox {
    display: flex;
    gap: 3rem;
    margin-left: 10rem;
    padding-top: 2rem;
}

span {
    font-size: 15px;
    font-weight: bolder;
    color: white;
}

ul,
a {
    font-size: 13px;
    text-decoration: none;
    list-style: none;
    color: rgb(151, 151, 151)
}

img {
    position: absolute;
    width: 30rem;
    top: -5.5rem;
    left: 47rem;
}
</style>