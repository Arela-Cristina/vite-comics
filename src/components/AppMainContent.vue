<!-- codice Javascript -->
<script>
import CardFumeti from './CardFumeti.vue';
import CardFumetti from './CardFumetti.vue';

export default {
    name: "AppMainContent",
    components: {
        CardFumeti,
        CardFumetti
    },
    data() {
        return {
            arrayComics: [
                {
                    "thumb": "https://m.media-amazon.com/images/I/61KFLylOgPL.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel",
                }
            ]
        }
    }
}

</script>

<!-- Codice HTML -->
<template>
    <section>
        <div class="currentSeries">CURRENT SERIES</div>
        <div id="jumbutron"></div>
        <div class="container-fumeti">
            <!-- <CardFumeti v-for="(CardFumeto, index) in arrayComics" :key="index" :details="CardFumeto"/> -->
            <CardFumetti v-for="(comic, index) in arrayComics" :key="index" :details="comic" />
        </div>
        <div class="loadMore">LOAD MORE</div>
    </section>
</template>

<!-- Codice Css -->
<style scoped>
#jumbutron {
    background-image: url(../../public/img/jumbotron.jpg);
    background-size: cover;
    width: 100%;
    height: 18rem;
}

section {
    background-color: rgb(24, 24, 24);
    padding-bottom: 1rem;
    position: relative;
}

.container-fumeti {
    width: 100%;
    min-height: 10rem;
    padding-left: 10rem;
    padding-right: 10rem;
    padding-top: 3rem;
    padding-bottom: 3rem;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    gap: 2rem;

}

.currentSeries {
    color: white;
    font-size: 17px;
    background-color: #0282f9;
    min-width: 15%;
    margin: 0 auto;
    padding: 10px 21px;
    position: absolute;
    font-weight: 900;
    top: 17rem;
    left: 10rem;
    text-align: center;
}

.loadMore {
    color: white;
    font-size: 12px;
    background-color: #0282f9;
    width: 10%;
    margin: 0 auto;
    padding: 10px 10px;
    text-align: center;
}
</style>