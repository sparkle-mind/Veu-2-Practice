<template>
    
    <div>
        <h2 v-once >{{name}}</h2>
        <h2>{{name}}</h2>

        <button v-on:click="nameChanged">click me</button>

        <br>
        <br>
        <hr>
        <br>
    </div>
</template>

<script>
export default{
    name:"vOnce",
    data(){
        return {
            name:"sam",
            age:24,
            ok:true
        }
    },
    methods:{
        nameChanged(){
                this.name="samir patel"
        }
    }
}
</script>


<!-- NOTE:
-> The v-once directive is used to only render an element once. 
By only rendering an element once, the performance can be enhanced. When an element has the v-once directive, all its child elements also becomes static after the first render. -->
