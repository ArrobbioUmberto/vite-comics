<script>
export default {

}
</script>
<template>
    <header>
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
    </header>
</template>

<style>
li {
    list-style-type: none;
    padding: 2px 10px;
    margin: 2px 5px;
    text-transform: uppercase;

}

li:hover {
    border-bottom: 2px solid blue;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

ul {
    display: flex;
}
</style>