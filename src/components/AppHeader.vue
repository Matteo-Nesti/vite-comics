<script>
export default {
    data() {
        return {
            links: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ],

        }

    },
    methods: {
        getActive(clickedLink) {
            this.links.forEach(link => {
                link.current = (link === clickedLink)
            });
        }
    }

}
</script>

<template>
    <header class="container">
        <figure>
            <img src="../assets/img/dc-logo.png" alt="">
        </figure>
        <nav>
            <ul>
                <li v-for="link in links">
                    <a :href="link.url" :key="link.text" :class="{ current: link.current }" @click="getActive(link)">{{ link.text }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;

    figure {
        width: 80px;
    }
}

ul {
    display: flex;

    li {
        margin: 0 15px;

        a {
            color: black;
            font-weight: 600;
            text-transform: uppercase;
            font-size: 0.9rem;
            padding-bottom: 36px;
        }
    }
}

a:hover,
a.current {
    color: #0282f9;
    border-bottom: 4px solid #0282f9;
}
</style>