<script>
export default {
    props: {
        thumbs: String,
        series: String,
    }
}
</script>
<template>
    <li>
        <img src="thumbs" alt="">
        <h3>{{ series }}</h3>
    </li>
</template>
<style lang="scss" scoped>
h3 {
    font-size: 10px;
}
</style>