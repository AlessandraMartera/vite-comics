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
        <img :src="details.thumb" :alt="details.series">
        <div>
            {{ details.series }}
        </div>
    </div>
</template>
  
<style lang="scss" scoped>
.card {
    width: 140px;
    height: 140px;

    img {
        width: 100%;
    }
}
</style>
  