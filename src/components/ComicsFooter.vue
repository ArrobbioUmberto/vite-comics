<script>
export default {
    data() {
        return {
            listMenufooter: [
                { menu: 'dc comics', text: 'characters', link: '#', },
                { menu: 'dc comics', text: 'comics', link: '#', },
                { menu: 'dc comics', text: 'movies', link: '#', },
                { menu: 'dc comics', text: 'tv', link: '#', },
                { menu: 'dc comics', text: 'games', link: '#', },
                { menu: 'dc comics', text: 'videos', link: '#', },
                { menu: 'dc comics', text: 'news', link: '#', },
                { menu: 'shop', text: 'shop dc', link: '#', },
                { menu: 'shop', text: 'shop dc collectibles', link: '#', },
                { menu: 'dc', text: 'terms of use', link: '#', },
                { menu: 'dc', text: 'privacy policiy (new)', link: '#', },
                { menu: 'dc', text: 'ad choice', link: '#', },
                { menu: 'dc', text: 'advertising', link: '#', },
                { menu: 'dc', text: 'jobs', link: '#', },
                { menu: 'dc', text: 'subscriptions', link: '#', },
                { menu: 'dc', text: 'talent workshops', link: '#', },
                { menu: 'dc', text: 'CPSC certificates', link: '#', },
                { menu: 'dc', text: 'ratings', link: '#', },
                { menu: 'dc', text: 'shop help', link: '#', },
                { menu: 'dc', text: 'contact us', link: '#', },
                { menu: 'sites', text: 'dc', link: '#', },
                { menu: 'sites', text: 'mad magazine', link: '#', },
                { menu: 'sites', text: 'dc kids', link: '#', },
                { menu: 'sites', text: 'dc universe', link: '#', },
                { menu: 'sites', text: 'dc power visa', link: '#', },
            ]
        }
    },
    methods: {

    },
    // uso il computed perche ho dati reattivi
    computed: {
        DcComicsMenu() {
            return this.listMenufooter.filter(el => {
                return el.menu === 'dc comics'
            })
        },
        ShopMenu() {
            return this.listMenufooter.filter(el => {
                return el.menu === 'shop'
            })
        },
        DcMenu() {
            return this.listMenufooter.filter(el => {
                return el.menu === 'dc'
            })
        },
        SitesMenu() {
            return this.listMenufooter.filter(el => {
                return el.menu === 'sites'
            })
        }
    }
}
</script>
<template>
    <footer>
        <section class="shop">
            <div class="container">
                <div class="row">
                    <div class="col">
                        <ul>
                            <li v-for="el in DcComicsMenu">
                                <a :href="el.link">{{ el.text }}</a>
                            </li>
                        </ul>
                        <ul>
                            <li v-for="el in ShopMenu">
                                <a :href="el.link">{{ el.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col">
                        <ul>
                            <li v-for="el in DcMenu">
                                <a :href="el.link">{{ el.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col">
                        <ul>
                            <li v-for="el in SitesMenu">
                                <a :href="el.link">{{ el.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="row">
                    <img src="/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </section>
        <section class=" social">
            <div class="container social">
                <div class="col">
                    <button>
                        SIGN UP NOW
                    </button>
                </div>
                <div class="col follow">
                    <h2>FOLLOW US</h2>
                    <ul class="logo">
                        <li><img src="/img/footer-facebook.png" alt=""></li>
                        <li><img src="/img/footer-twitter.png" alt=""></li>
                        <li><img src="/img/footer-youtube.png" alt=""></li>
                        <li><img src="/img/footer-pinterest.png" alt=""></li>
                        <li><img src="/img/footer-periscope.png" alt=""></li>
                    </ul>
                </div>
            </div>
        </section>

    </footer>
</template>

<style>
footer {
    background-image: url('/img/footer-bg.jpg');
}


footer li {
    color: white;
    list-style-type: none;
    text-align: start;
    font-weight: 300;
}

footer .shop li:first-child {
    text-transform: uppercase;
    font-weight: bold;
    padding: 15px 0;
}

footer .row {
    display: flex;
    flex-direction: row;
}

footer .container {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    max-width: 1280px;
    margin: 0 auto;
    position: relative;
    padding: 40px 0;
}

footer .shop img {
    position: absolute;
    right: 0%;
    top: -20%;
}

footer button {
    color: white;
    border: 1px solid cornflowerblue;
    border-radius: 0;
    background-color: #303030;
}

.container.social {
    justify-content: space-between;
    padding: 15px 0;
}

.social {
    background-color: #303030;
}

.follow {
    display: flex;
    flex-direction: row;
}

.logo {
    display: flex;
    flex-direction: row;
}

.logo li {
    padding: 10px;
}
</style>