<script>
import ComicsCard from './ComicsCard.vue';
export default {
    components: {
        ComicsCard
    },
    data() {
        return {
            ServiceList: [
                { icon: '/img/buy-comics-digital-comics.png', text: 'digital comics' },
                { icon: '/img/buy-comics-merchandise.png', text: 'dc merchandise' },
                { icon: '/img/buy-comics-subscriptions.png', text: 'subscription' },
                { icon: '/img/buy-comics-shop-locator.png', text: 'comic shop locator' },
                { icon: '/img/buy-dc-power-visa.svg', text: 'dc power visa' }
            ],

            Comics: [
                {
                    thumb: "./img/copertina1.jpg",
                    price: "$19.99",
                    series: "Action Comics",
                    type: "comic book"
                },
                {
                    thumb: "./img/copertina2.jpg",
                    price: "$3.99",
                    series: "American Vampire 1976",
                    type: "comic book"
                },
                {
                    thumb: "./img/copertina3.jpg",
                    price: "$16.99",
                    series: "Aquaman",
                    type: "graphic novel"
                },
                {
                    thumb: "./img/copertina4.jpg",
                    price: "$2.99",
                    series: "Batgirl",
                    type: "comic book"
                },
                {
                    thumb: "./img/copertina5.jpg",
                    price: "$3.99",
                    series: "Batman",
                    type: "comic book"
                },
                {
                    thumb: "./img/copertina6.jpg",
                    price: "$2.99",
                    series: "Batman Beyond",
                    type: "comic book"
                },
                {
                    thumb: "./img/copertina7.jpg",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book"
                },
                {
                    thumb: "./img/copertina8.jpg",
                    price: "$4.99",
                    series: "Batman / Superman Annual",
                    type: "comic book"
                },
                {
                    thumb: "./img/copertina9.jpg",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book"
                },
                {
                    thumb: "./img/copertina10.jpg",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book"
                },
                {
                    thumb: "./img/copertina11.jpg",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book"
                },
                {
                    thumb: "./img/copertina12.jpg",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel"
                }
            ]
        }
    },
    methods: {

    }
}
</script>
<template>
    <main>
        <section class="content">
            <div class="container">
                <ul>
                    <ComicsCard v-for="(el, i) in Comics" :key="i" :thumb="el.thumb" :series="el.series">
                    </ComicsCard>
                </ul>
            </div>
        </section>
        <section class="blue-stripe">
            <div class="container">
                <div>
                    <ul>
                        <li v-for="service in ServiceList">
                            <img :src="service.icon" alt="">{{ service.text }}
                        </li>
                    </ul>
                </div>
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables.scss' as *;

main {
    background-color: $dc-blue;
}

.container {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    max-width: 1280px;
    margin: 0 auto;
}

.content {
    background-color: black;
}

h1 {
    color: white;
    padding: 40px;
    font-size: 25px;
}

ul {
    display: flex;
    justify-content: space-around;
    align-items: center;
}

li {
    color: white;
    display: flex;
    align-items: center;
    list-style-type: none;
    text-transform: uppercase;
    margin: 0 10px;
    font-family: 'Times New Roman', Times, serif;
}

li:nth-child(4) img {
    width: 50px;
}

li:first-child img {
    width: 50px;
}

img {
    width: 60px;
    padding: 0 10px;
}


.blue-stripe {
    padding: 40px 0;
}
</style>