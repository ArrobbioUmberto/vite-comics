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
    padding: 2px 10px;
    margin: 2px 5px;
    text-transform: uppercase;

}

header li:hover {
    border-bottom: 2px solid blue;
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
}
</style>