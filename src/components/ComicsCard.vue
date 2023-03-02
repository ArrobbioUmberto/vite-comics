<script>
export default {
    props: {
        thumb: String,
        series: String,
    }
}
</script>
<template>
    <li>
        <img :src="thumb" alt="">
        <h3>{{ series }}</h3>
    </li>
</template>
<style lang="scss" scoped>
h3 {
    font-size: 20px;
    margin: 5px 0;
}

li {
    display: flex;
    flex-direction: column;
    flex-basis: calc((100% / 7) - 10px);
    align-items: center;
    justify-content: center;
}

li:last-child {
    padding: 0;
}

img {
    width: 100%;
    aspect-ratio: 3/4;
}
</style>