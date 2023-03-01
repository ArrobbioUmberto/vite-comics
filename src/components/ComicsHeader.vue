<script>
export default {

}
</script>
<template>
    <header>
        <div class="container">
            <div>
                <img src="/img/dc-logo.png" alt="">
            </div>
            <ul>
                <li>characters</li>
                <li>comics</li>
                <li>movies</li>
                <li>tv</li>
                <li>games</li>
                <li>collectibles</li>
                <li>videos</li>
                <li>fans</li>
                <li>news</li>
                <li>shop</li>
            </ul>
        </div>
    </header>
</template>

<style>
header li {
    color: black;
    list-style-type: none;
    padding: 50px 10px;
    text-transform: uppercase;
    box-sizing: border-box;
    border-bottom: 5px solid transparent;
}

header li:hover {
    border-bottom-color: blue;
}

.container {
    display: flex;
    justify-content: space-around;
    align-items: center;
    max-width: 1280px;
    margin: 0 auto;
}

header ul {
    display: flex;
    padding-inline-start: 0;
    margin-block: 0;
}
</style>