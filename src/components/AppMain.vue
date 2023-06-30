<script>
import AppCards from './AppCards.vue'
export default {
    components: { AppCards },
    data() {
        return {

        }
    },
    props: {
        mainCards: Array
    }

}
</script>

<template>
    <main>
        <section id="jumbo">
            <img src="https://static.dc.com/2023-06/DC.com_20230629_HL_ComingOut_Marquee_3x1_.jpg?w=1200" alt="Losing the Mask: Five Comic Book Coming Out Stories">
            <div class="container">
                <a href="#" class="jumbo-btn">current Series</a>
            </div>
        </section>
        <section id="mainContent" class="container">
            <AppCards :mainCards="mainCards" />
            <div class="btn-main">
                <a href="#">LOAD MORE</a>
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
main {
    background-color: black;


    p {
        font-size: 1.5rem;
        color: #fff;
        padding: 80px 20px;
    }

}

#jumbo {
    img {
        width: 100%;
    }

    .jumbo-btn {
        color: #FFF;
        background-color: #0282f9;
        font-size: 1.3rem;
        padding: 10px 20px;
        position: relative;
        bottom: 35px;

    }

}

.btn-main {
    display: flex;
    justify-content: center;

}

a {
    color: #FFF;
    font-weight: bold;
    background-color: #0282f9;
    padding: .7rem 1.8rem;
    display: inline-block;
    margin: 10px auto;
    cursor: pointer;
    transition: .3s;
}

a:hover {

    scale: 1.1;
}
</style>