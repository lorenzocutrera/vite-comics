<script>

export default {
    name: 'appMain'
}
</script>

<template>
    <div class="menu d-flex">
        <div class="container">
            <div class="row d-flex">

                <div class="col">
                    <div class="option d-flex">
                        <img src="../assets/comics-img/img/buy-comics-digital-comics.png" alt="">
                        <p class="d-flex">DIGITAL COMICS</p>
                    </div>
                </div>

                <div class="col">
                    <div class="option d-flex">
                        <img src="../assets/comics-img/img/buy-comics-merchandise.png" alt="">
                        <p class="d-flex">DIGITAL COMICS</p>
                    </div>
                    
                </div>

                <div class="col">
                    <div class="option d-flex">
                        <img src="../assets/comics-img/img/buy-comics-subscriptions.png" alt="">
                        <p class="d-flex">DIGITAL COMICS</p>
                    </div>
                    
                </div>

                <div class="col">
                    <div class="option d-flex">
                        <img src="../assets/comics-img/img/buy-comics-shop-locator.png" alt="">
                        <p class="d-flex">DIGITAL COMICS</p>
                    </div>
                    
                </div>

                <div class="col">
                    <div class="option d-flex">
                        <img src="../assets/comics-img/img/buy-dc-power-visa.svg" alt="">
                        <p class="d-flex">DIGITAL COMICS</p>
                    </div>
                    
                </div>
            </div>
        </div>
    </div>

    <div class="main">
        <div class="container">

        </div>
    </div>
</template>

<style lang="scss">
.menu {
    height: 150px;
    width: 100%;
    background-color: #0182fa;


}

.main {
    width: 100%;
    height: calc(100vh - 500px);
    background-image: url(../assets/comics-img/img/footer-bg.jpg);

}

.option {

    p {
        color: white;
        align-items: center;
        font-size: 15px;
        padding: 5px;
    }

    img{
        width: 30%;
    }

}
</style>