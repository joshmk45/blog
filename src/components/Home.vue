<template>
    <div>
        <h1>template in vue.js</h1>
        <h2>{{ name }}</h2>
        <button v-on:click="count">click</button>
    </div>
</template>

<script>
export default{
    name:"HomePage",
    data(){
        return {
            name:"mwanuke"
        }
    
       },methods:{
            count(){
                if(this.name=="joseph"){
                    this.name="mwanuke";
                }
                else{
                    this.name="joseph"; 
                }
            }
}
}

</script>