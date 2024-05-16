<template>
    <div>
        <h2 v-if="show">if statement</h2>
        <h2 v-else>Else statement</h2>
        <button v-on:click="btnClick"> click me</button>
        <br>
        <br>
        <hr>
        <br>
    </div>
</template>
<script>
export default{
    name:"IfElse",
    data(){
        return {
            show:true  // if this value is true then print show "if statement"
            // show:false  // if this value is false then print show "else statement"
        }
    },
    methods:{
        btnClick(){
            this.show = !this.show; // toggle the value of show
            console.log("btn was clicked");
            
        }
    }
}
</script>

<style scoped>
h2{
    color:brown;
    text-transform: uppercase;
}

</style>

<!-- 

Note:

-> make sure if elements are one than more then wrap all element in  <div> <div/>  ---- template
-> if /else condition must be write in data() function.
-> scoped : if we write scoped in style it means this css will apply only this component.
-> event or methods/function must be write in method: 







-->