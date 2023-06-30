<script>
export default {
    props: {
        mainCards: Array,
    }
}
</script>

<template>
    <div class="container container-card">
        <div class="card" v-for="card in mainCards">
            <img :src="card.thumb" alt="">
            <h4>{{ card.series }}</h4>
        </div>
    </div>
</template>

<style scoped lang="scss">
.container-card {
    padding: 2rem 0;
    display: flex;
    flex-wrap: wrap;
}

.card {
    width: calc(100% / 6);
    padding: .6rem;
    opacity: .8;
    transition: scale .3s;
    text-align: center;

    img {
        width: 150px;
        height: 150px;
        object-fit: cover;
        object-position: top;
    }

    h4 {
        color: #fff;
        margin: 1rem .5rem;
    }
}

.card:hover {
    scale: 1.1;
    cursor: pointer;
    opacity: 1;
}
</style>