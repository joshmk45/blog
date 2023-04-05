<template>
<div>
<!-- <h1>hello from home component</h1>
<h1>{{username}}</h1>
<h1>{{msg}}</h1>
<button v-on:mouseover="hello('username')">call hello function</button> -->
<!-- <h1 v-if="show">conditional rendering in vue.js</h1>
<h1 v-else>else side of above</h1> -->
<!-- <button v-on:click="showFunction">Toggle</button> -->
<h1>for loop in vue.js</h1>
<table>
    <tr>
        <th>ID</th><th>NAME</th><th>EMAIL</th>
    </tr>
    <tr v-for="user in users" :key="user.id">
    <td>{{user.id}}</td>
    <td>{{user.name}}</td>
    <td>{{user.email}}</td>
    </tr> 
</table>
</div>

    
</template>
<script>
export default{
    name:'HomePage',
    props:{
        username:String,
        msg:String
    },methods:{
        //method with parameter
        hello(data)
        {
            alert("clicked "+data);
        },
        //method without parameter
        showFunction(){
            this.show=!this.show
        }

    },data()
    {
        //data used for condition used in template
        // return{
        //     show:false
        // }
        return{
            users:[
                {id:1,name:"jose",email:"mkjosh501@gmail.com"},
                {id:2,name:"toly",email:"mkjosh501@gmail.com"},
                {id:3,name:"adi",email:"mkjosh501@gmail.com"},
                {id:4,name:"part",email:"mkjosh501@gmail.com"},
            ]
        }
    },
}
</script>
<style>
 /* h1{
    color:red;
    text-align: left;
    margin: 0;
 } */
 table{
    margin:auto;
 }
</style>