<template>
    <div>
        <h2 v-if="condition === 'A'">Condition A is true</h2>
        <h2 v-else-if="condition === 'B'">Condition B is true</h2>
        <h2 v-else>Neither condition A nor B is true</h2>

        <br>
        <br>
        <hr>
        <br>
    </div>
</template>

<script>
export default {
    name: "elseIf",
    data() {
        return {
            // condition: 'A' // Change this value to 'B' or anything else to see different conditions
            // condition: 'B' // Change this value to 'B' or anything else to see different conditions
            condition: 'C' // Change this value to 'B' or anything else to see different conditions
        }
    }
}
</script>