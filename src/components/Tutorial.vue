<template>
    <h1>Home Component {{ "helloworld".length }}</h1>
    <h2 v-on:mousemove="getConsole()">Mouse move</h2>
    <h2>{{ count }}</h2>
    <!-- <h2>Email: {{email}}</h2>
    <h2>Name: {{getName()}}</h2>
    <h2>Data: {{getData().email}}</h2> -->
    <button v-on:click="changeValue()">Increase Value</button>
    <button v-on:click="getData()">Decrease Value</button>
    <button v-on:dblclick="doubleClick('button 2 clicked')">Double Click</button>
</template>

<script>
export default {
    // name: "Home",
    // data(){
    //     return{
    //         email:"testmail.com"
    //     }
    // },
    data(){
        return{
            count:0
        }
    },
    methods:{
        getData()
        {
            this.count=this.count-1
        },
        changeValue()
        {
            this.count=this.count+1
        },
        doubleClick(data)
        {
            alert(data)
        },
        getConsole(){
            console.log("event is fired")
        }
    }
}
</script>

<style scoped>
h1 {
    color:orange
}
</style>