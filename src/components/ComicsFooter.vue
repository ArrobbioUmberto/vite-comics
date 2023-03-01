<script>
export default {

}
</script>
<template>
    <footer>
        <section class="shop">
            <div class="container">
                <div class="row">
                    <div class="col">
                        <ul>
                            <li>dc comics</li>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>Tv</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <ul>
                            <li>shop</li>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                    <div class="col">
                        <ul>
                            <li>dc</li>
                            <li>Term of Use</li>
                            <li>Privacy policy(New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certficates </li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>
                    <div class="col">
                        <ul>
                            <li>sites</li>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
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