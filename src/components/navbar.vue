<script>

export default {
    name: 'navbar',
    data() {
        return{
           navbar : ['CHARACTERS', 'COMICS', 'MOVIES','TV','GAMES','COLLECTIBLES','VIDEOS','FANS','NEWS','SHOP']
        } 
        
    }


}



</script>


<template>
    <nav class="d-flex">
        <div v-for="item in navbar" class="nav-item">
            <a href="#">{{ item }}</a>
        </div>
    </nav>
</template>

<style lang="scss">
.nav-item{
    height: 100%;
}

</style>