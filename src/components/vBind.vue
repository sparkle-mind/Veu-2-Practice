<template>
    <div>
        <h2>v-bind:src for imgs</h2>
        <img v-bind:src="url">
        <br>
        <br>
        <hr>
        <h2>v-bind:style for inline css</h2>
        <h3 v-bind:style="{color:textColor, fontSize:fSize}">this is inline style</h3>
        <h3 v-bind:style="{fontSize:fSize2 + 'px'}">this is inline style 2</h3>
        <br>
        <br>
        <hr>
        <h2>JavaScript conditional (ternary) expression</h2>
        <div v-bind:style="{ backgroundColor: isImportant ? 'green' : 'yellow' }">
            Conditional background color
        </div>
        <br>
        <br>
        <hr>
        <h2>className</h2>
        <div v-bind:class="classAdded">
            The class is set with Vue
        </div>
        <br>
        <br>
        <hr>
        <div v-bind:class="{ myClass: true }">
             The class is set conditionally to change the background color
        </div>
        <br>
        <br>
        <hr>
        <div v-bind:class="{ myClass2: isAvailable }">
            The class is set conditionally to change the background color
        </div>
        <br>
        <br>
        <hr>
 
    </div>
</template>

<script>
export default{
    name:"vBind",
    data(){
        return{
            url:"https://images.pexels.com/photos/23719481/pexels-photo-23719481/free-photo-of-chrysanthemum-flower.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load",
            textColor:"red",
            fSize:"32px",
            fSize2:50,
            // isImportant:true,
            isImportant:false,
            classAdded:"addClass",
            isAvailable:true
        }
    }
   
}
</script>


<style scoped>
.addClass{
    font-size: 30px;
    color:blueviolet;
}
.myClass{
    color: rgb(4, 192, 82);
}
.myClass2{
    background-color: red;
    padding: 10px;
    color: #fff;
}
</style>