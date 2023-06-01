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

        <div class="title_card">
            {{ details.series }}
        </div>
    </div>
</template>
  
<style lang="scss" scoped>
.card {
    width: calc((100% / 6) - 10px);

    img {
        width: 100%;
        aspect-ratio: 1 / 1;
    }

    .title_card {
        margin-top: 5px
    }
}
</style>
  