<script>
export default {

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
                        <li><img src="/img/buy-comics-digital-comics.png" alt=""> digital comics</li>
                        <li><img src="/img/buy-comics-merchandise.png" alt=""> dc merchandise</li>
                        <li><img src="/img/buy-comics-subscriptions.png" alt=""> subscription</li>
                        <li><img src="/img/buy-comics-shop-locator.png" alt="" id="locator-img"> comic shop locator</li>
                        <li><img src="/img/buy-dc-power-visa.svg" alt=""> dc power visa</li>
                    </ul>
                </div>
            </div>
        </section>
    </main>
</template>

<style>
main {
    background-color: #0282f9;
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
    padding: 0 10px;
}

#locator-img {
    width: 40px;
}

main .blue-stripe {
    padding: 40px 0;
}
</style>