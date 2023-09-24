<script>


export default {
    Name: 'appFooter',
    data() {
        return {
            menuFooter: [
                {
                    title: 'DC COMICS',
                    elements: ['Characters', 'comics', 'movies', 'TV', 'Games', 'Videos', 'News']
                },
                {
                    title: 'SHOP',
                    elements: ['Shop DC', 'Shop DC collectibles']
                },
                {
                    title: 'DC',
                    elements: ['Terms of Use', 'Privacy policy(new)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscription', 'Talent Workshop', 'CPSC Certificate', 'Ratings', 'Shop Help', 'Contact Us']
                },
                {
                    title: 'SITES',
                    elements: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
                },
            ],

            socials: ['src/assets/comics-img/img/footer-facebook.png', 'src/assets/comics-img/img/footer-twitter.png', 'src/assets/comics-img/img/footer-youtube.png', 'src/assets/comics-img/img/footer-pinterest.png', 'src/assets/comics-img/img/footer-periscope.png']
        }

    }

};
</script>

<template>
    <div class="main_footer">
        <div class="container d-flex">
            <div class="liste d-flex">
                <ul v-for="liste in menuFooter" class="menuFooter">
                    <li>{{ liste.title }}
                        <ul v-for="item in liste.elements">
                            <li><a href="#">{{ item }}</a></li>
                        </ul>
                    </li>
                </ul>
            </div>

            <div class="mainDC">
                <img src="../assets/comics-img/img/dc-logo-bg.png" alt="">
            </div>
     </div>
    </div>
    <footer>
        <div class="container">
            <div class="riga d-flex">
                <div class="button">
                    <button>SIGN-UP NOW!</button>
                </div>

                <div class="socials d-flex">
                    <h4>FOLLOW US</h4>
                    <div v-for="social in socials" class="social d-flex">
                        <img :src="social" alt="">
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss">
.main_footer {
    width: 100%;
    height: calc(100vh - 500px);
    background-image: url(../assets/comics-img/img/footer-bg.jpg);
    color: white;
}

ul {
    list-style: none;

    a {
        text-decoration: none;
        color: #797979;
    }
}

.menuFooter {
    display: flex;
    flex-wrap: wrap;
}

footer {
    width: 100%;
    height: 100px;
    background-color: #303030;
    display: flex;
    align-items: center;
}

.riga {
    justify-content: space-between;
    align-items: center;
}

button {
    background-color: #303030;
    color: #fff;
    border: solid #0182fa;
    padding: 5px 5px;
}

.socials {
    h4 {
        color: #0182fa;
        margin: 10px;
    }

    img {
        padding: 10px;
    }
}</style>