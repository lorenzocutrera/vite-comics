<script>


export default {
    name: 'appHeader'
}
</script>

<template>
    <div class="top d-flex">
        <div class="container">
            <div class="row d-flex">
                <div class="col">
                    <img src="../assets/comics-img/img/dc-logo.png" alt="">
                </div>
                <div class="col">
                    <a href="#">characters</a>
                    <a href="#">comics</a>
                    <a href="#">movie</a>
                    <a href="#">tv</a>
                    <a href="#">games</a>
                    <a href="#">collectibles</a>
                    <a href="#">videos</a>
                    <a href="#">fans</a>
                    <a href="#">news</a>
                    <a href="#">shop</a>
                </div>
            </div>
        </div>
    </div>

    <div class="bottom d-flex">
        <div class="container">
            <h3 style="color:white; font-size: 20px;"> -->Content goes here -- </h3>
        </div>
    </div>
</template>

<style lang="scss">
.top {
    height: 100px;
    width: 100%;
    background-color: #fff;
}


.row {
    height: 100%;
    align-items: center;
    justify-content: space-between;
}

.col {
    display: flex;

    img {
        width: 80px;
    }

    a {
        text-decoration: none;
        color: black;
        margin: auto 10px;
    }
}

.bottom {
    align-items: center;
    height: 100px;
    width: 100%;
    background-color: black;

    
}

h3{
font-size: 10px;
}
    

</style>