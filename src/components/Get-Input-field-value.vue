<template>
    <h1>Get Input field value</h1>
    <input type="text" placeholder="Enter Email" v-model="email" />
    <br><br>
    <input type="password" placeholder="Enter password" v-model="password" />
    <br><br>
    <button type="button" v-on:click="getData()">Get Data</button>
</template>

<script>
export default {
    name: "Home",
    data()
    {
        return{
            email:null,
            password:null
        }
    },
    methods:{
        getData()
        {
            console.warn("values:" , this.email, this.password);
        }
    }
}
</script>

<style scoped>
h1 {
    color:orange
}
</style>