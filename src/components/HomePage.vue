<template>
    <div class="home">
        <h1>this is Home component</h1>
        <userPage/>
        <productPage/>

    </div>
</template>
<script>
import userPage from './userPage.vue'
import productPage from './productsPage.vue'
export default {
    name:"HomePage",
    components:{
        userPage,
        productPage
    }
}
</script>
<style>
.home{
    margin-top:0;
    height:500px;
    background-color:aquamarine;
    text-align: center;
}
</style>