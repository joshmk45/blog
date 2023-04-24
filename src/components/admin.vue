<template>
    <div class="admin">
        <h1>Admin</h1> 
        <ProductPage/>
        <UserPage/>
    </div>
    
</template>

<script>
import ProductPage from './Products.vue';
import UserPage from './Users.vue';
export default({
    name:"AdminPage",
    components:{
        ProductPage,
        UserPage
    }
})
</script>
<style>
.admin{
    background-color:#09036f;
    height:500px;
    padding:20px;
}
</style>
