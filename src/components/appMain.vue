<script>

export default {
    name: 'appMain',
    data() {
        return{
           menu : [
            {
                image: "/src/assets/comics-img/img/buy-comics-digital-comics.png",
                title: 'DIGITAL COMICS'
            },
            {
                image: "/src/assets/comics-img/img/buy-comics-merchandise.png",
                title: 'DC MERCHANDISE'
            },
            {
                image: "/src/assets/comics-img/img/buy-comics-subscriptions.png" ,
                title: 'SUBSCRIPTION'
            },
            {
                image: "/src/assets/comics-img/img/buy-comics-shop-locator.png"  ,
                title: 'COMIC SHOP LOCATOR'
            },
            {
                image: "/src/assets/comics-img/img/buy-dc-power-visa.svg" ,
                title: 'DC POWER VISA'
            },
           ]
        } 
        
    }

}
</script>

<template>
     <div class="bottom d-flex">
        <div class="container">
            <h3 style="color:white; font-size: 20px;"> -->Content goes here -- </h3>
        </div>
    </div>
    <!-- menu -->
    <div class="menu d-flex">
        <div class="container">
            
            <div  class="row d-flex">

                <div v-for="item in menu" class="col">
                    <div class="option d-flex">
                        <img v-bind:src="item.image" alt="">
                
                        <p class="d-flex">{{item.title}}</p>
                    </div>
                </div>

            </div>
        </div>
    </div>

   
</template>

<style lang="scss">
.menu {
    height: 150px;
    width: 100%;
    background-color: #0182fa;


}

.bottom {
    align-items: center;
    height: 150px;
    width: 100%;
    background-color: black;

    
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