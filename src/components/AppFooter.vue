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
    }
}
</script>

<template>
    <footer>
        <section id="linkSection">
            <div class="container d-flex">

                <div>
                    <h3>DC COMICS</h3>
                    <ul>
                        <li v-for="link in links">
                            <a href="link.url">{{ link.text }}</a>
                        </li>
                    </ul>

                    <h3>SHOP</h3>
                    <ul>
                        <li>
                            <a href="#">Shop Dc</a>
                        </li>

                        <li>
                            <a href="#">Shop Dc Collection</a>
                        </li>
                    </ul>
                </div>

                <div>
                    <h3>DC</h3>
                    <ul>
                        <li>
                            <a href="#">Terms of Use</a>
                        </li>
                        <li>
                            <a href="#">Privacy Policy</a>
                        </li>
                        <li>
                            <a href="#">Ad Choices</a>
                        </li>
                        <li>
                            <a href="#">Advertising</a>
                        </li>
                        <li>
                            <a href="#">Jobs</a>
                        </li>
                        <li>
                            <a href="#">Subscriptions</a>
                        </li>
                        <li>
                            <a href="#">Talent Workshopos</a>
                        </li>
                        <li>
                            <a href="#">CPSC Certificates</a>
                        </li>
                        <li>
                            <a href="#">Ratings</a>
                        </li>
                        <li>
                            <a href="#">Shop Help</a>
                        </li>
                        <li>
                            <a href="#">Contact Us</a>
                        </li>
                    </ul>
                </div>

                <div>
                    <h3>SITES</h3>
                    <ul>
                        <li>
                            <a href="#">DC</a>
                        </li>
                        <li>
                            <a href="#">MAD Magazine</a>
                        </li>
                        <li>
                            <a href="#">DC Kids</a>
                        </li>
                        <li>
                            <a href="#">DC Universe</a>
                        </li>
                        <li>
                            <a href="#">DC Power Visa</a>
                        </li>
                    </ul>
                </div>

            </div>

        </section>

        <section id="socialSection">
            <div class="container contactLinks">
                <div>
                    <a class="btn" href="#">SIGN UP NOW!</a>
                </div>
                <div class="d-flex">
                    <h4>FOLLOW US</h4>
                    <a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a>
                </div>
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
footer {
    background-image: url('../assets/img/footer-bg.jpg');

    background-size: cover;
}

#linkSection {
    padding: 30px 0;
    background-image: url('../assets/img/dc-logo-bg.png');
    background-repeat: no-repeat;
    background-position: 800px;

    h3 {
        color: white;
        margin: 10px 0;
    }

    a {
        color: gray;
        font-size: .8rem;
    }

    a:hover {
        color: lightgrey;
    }


}

#socialSection {
    background-color: #303030;
    padding: 20px 0;

    a.btn {
        color: #fff;
        padding: 10px 20px;
        border: 2px solid#0282f9;
        transition: .3s;
    }

    a.btn:hover {
        background-color: #0282f9;
        scale: 1.1;
    }

    h4 {
        color: #0282f9;
        font-size: 1.5rem;
        margin: 0 10px;
    }

    a {
        margin: 0 5px;
    }

    .contactLinks {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
}

.d-flex {
    display: flex;

    div {
        margin: 0 20px;
    }
}
</style>