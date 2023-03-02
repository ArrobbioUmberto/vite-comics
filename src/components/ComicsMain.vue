<script>
export default {
    data() {
        return {
            ServiceList: [
                { icon: '/img/buy-comics-digital-comics.png', text: 'digital comics' },
                { icon: '/img/buy-comics-merchandise.png', text: 'dc merchandise' },
                { icon: '/img/buy-comics-subscriptions.png', text: 'subscription' },
                { icon: '/img/buy-comics-shop-locator.png', text: 'comic shop locator' },
                { icon: '/img/buy-dc-power-visa.svg', text: 'dc power visa' }
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
                <h1>--> Content goes here &lt;--</h1>
            </div>
        </section>
        <section class="blue-stripe">
            <div class="container">
                <div>
                    <ul>
                        <li v-for="service in ServiceList">
                            <img src="service.icon" alt="">{{ service.text }}
                        </li>
                    </ul>
                </div>
            </div>
        </section>
    </main>
</template>

<style lang="scss">
@use '../style/partials/variables.scss' as *;

main {
    background-color: $dc-blue;
}

.content .container {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    max-width: 1280px;
}

.content {
    background-color: black;
}

main h1 {
    color: white;
    padding: 40px;
    font-size: 25px;
}

main ul {
    display: flex;
    justify-content: space-around;
    align-items: center;
}

main li {
    color: white;
    display: flex;
    align-items: center;
    list-style-type: none;
    text-transform: uppercase;
    margin: 0 10px;
    font-family: 'Times New Roman', Times, serif;
}

main img {
    width: 70px;
    height: 70px;
    padding: 0 10px;
}

#locator-img {
    width: 40px;
}

main .blue-stripe {
    padding: 40px 0;
}
</style>