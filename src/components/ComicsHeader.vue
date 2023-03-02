<script>
export default {
    data() {
        return {
            HeaderMenuList: [
                { text: 'characters', link: '#' },
                { text: 'comics', link: '#' },
                { text: 'movies', link: '#' },
                { text: 'tv', link: '#' },
                { text: 'games', link: '#' },
                { text: 'collectibles', link: '#' },
                { text: 'videos', link: '#' },
                { text: 'fans', link: '#' },
                { text: 'news', link: '#' },
                { text: 'shop', link: '#' },
            ]
        }
    }
}
</script>
<template>
    <header>
        <div class="container">
            <div>
                <img src="/img/dc-logo.png" alt="">
            </div>
            <ul>
                <li v-for="el in HeaderMenuList">
                    <a href="#">{{ el.text }}</a>
                </li>
            </ul>
        </div>
    </header>
</template>

<style lang="scss" scoped>
li {
    color: black;
    list-style-type: none;
    padding: 50px 10px;
    text-transform: uppercase;
    box-sizing: border-box;
    border-bottom: 5px solid transparent;
}

a {
    color: black;
}

li:hover {
    border-bottom-color: blue;
}

.container {
    display: flex;
    justify-content: space-around;
    align-items: center;
    max-width: 1280px;
    margin: 0 auto;
}

img {
    user-select: none;
}

ul {
    display: flex;
    padding-inline-start: 0;
    margin-block: 0;
}
</style>