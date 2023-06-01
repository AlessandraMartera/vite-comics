<script>
export default {
    name: 'productCard',
    props: {
        details: Object
    }
}

</script>

<template>
    <div class="card">
        <div>
            <img :src="details.thumb" :alt="details.series">
        </div>

        <div>
            {{ details.series }}
        </div>
    </div>
</template>
  
<style lang="scss" scoped>
.card {
    width: calc((100% / 6) - 10px);
    height: 140px;

    img {
        width: 100%;

    }
}
</style>
  