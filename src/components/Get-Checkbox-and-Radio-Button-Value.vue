<template>
    <h1>Get Checkbox and Radio Button Value</h1>
    <h3>Technology</h3>
    <label for="java">Java</label>
    <input type="checkbox" value="java" id="java" v-model="technology" />
    <label for="node">Node</label>
    <input type="checkbox" value="node" id="node" v-model="technology" />
    <label for="php">PHP</label>
    <input type="checkbox" value="php" id="php" v-model="technology" />
    
    <br><br>
    <h3>Profession</h3>
    <label for="student">Student</label>
    <input type="radio" value="student" id="student" v-model="profession" name="profession" />
    <label for="developer">Developer</label>
    <input type="radio" value="developer" id="developer" v-model="profession" name="profession" />
    <h4>Technology : {{technology}}</h4>
    <h4>I am a : {{profession}}</h4>
</template>

<script>
export default {
    name: "Home",
    data()
    {
        return{
            technology:[],
            profession:null
        }
    }
}
</script>

<style scoped>
h1 {
    color:orange
}
</style>