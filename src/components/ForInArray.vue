<template>
    <div>
        <h2>For-In Loop Demo -Array</h2>
            <ul>
                <li v-for="fruit in fruits" :key="fruit">{{ fruit }}</li>
            </ul>

        <br>
        <br>
        <hr>
        <br>
    </div>

</template>

<script>
export default {
    name: "ForInArray",
    data() {
        return {
            fruits: ['Apple', 'Banana', 'Orange', 'Mango',500,200] // Array of items to iterate over
        }
    }
}
</script>

<style scoped>
ul li {
    margin: 5px 0;
    padding: 0;
    text-align: left;
    text-transform: capitalize;
}
</style>