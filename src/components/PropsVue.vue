<template>
    <div>
        <h1>{{ myData1 }}</h1>  
        <h1>{{ myData2 }}   {{ samData }}</h1>  
        <h2>{{ 5+3 }}</h2>
        <h5>{{ samData }}</h5>
        <br>
        <br>
        <hr>
        <br>
    </div>
</template>

<script>
export default{
    name: "PropsVue",
    props:{
        myData1:String,
        myData2:String,
        samData:String
    }
}
</script>

<style>

</style>