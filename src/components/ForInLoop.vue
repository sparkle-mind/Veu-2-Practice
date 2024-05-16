<template>
    <div>
        <h2>For-In Loop Demo Array In Object</h2>
        <table>
            <tr>
                <td>id</td>
                <td>name</td>
                <td>email</td>
            </tr>
            <tr v-for="data in myData" :key="data">
                <td>{{ data.id }}</td>
                <td>{{ data.name }}</td>
                <td>{{ data.email }}</td>
            </tr>
        </table>
        <br>
        <br>
        <hr>
        <br>
    </div>
</template>
<script>
export default{
    name:"ForInLoop",
    data(){
        return{
            myData:[
                {id:1,name:"samir",email:"sam@gmail.com"},
                {id:2,name:"umang",email:"umang@gmail.com"},
                {id:3,name:"rinkesh",email:"rinkesh@gmail.com"}
            ]
        }
    }
}
</script>

<style scoped>
tr,td{
    border: 1px solid green;
    text-align: left;
    padding: 5px 20px;
}
</style>