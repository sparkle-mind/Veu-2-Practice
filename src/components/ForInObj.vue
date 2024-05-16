<template>
    <div>
        <h2>For-In Loop Demo -Object</h2>
        <ul>
            <li v-for="(value, key) in myObject" :key="key">
                {{ key }}: {{ value }}
            </li>
        </ul>

        <br>
        <br>
        <hr>
        <br>
    </div>

</template>

<script>
export default {
    name: "ForInObj",
    data() {
        return {
            myObject: {
                name: 'John Doe',
                age: 30,
                occupation: 'Developer'
            }
        };
    }
}
</script>

<style scoped>
ul li{
margin:5px 0;
padding: 0;
text-align: left;
text-transform: capitalize;
}
</style>