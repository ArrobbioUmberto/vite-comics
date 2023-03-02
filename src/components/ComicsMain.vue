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
                    "thumb": "./img/copertina1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
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
                    <ComicsCard v-for="(el, i) in Comics" :key="i" :thumbs="el.thumbs" :series="el.series">
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