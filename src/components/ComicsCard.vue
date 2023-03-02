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
    font-size: 10px;
}

img {
    width: 50px;
    height: 50px;
}
</style>