<template>
    <div>
        <h2>Ternory Operator</h2>

        <h3>{{ myData.ok ? "yes" : "no" }}</h3>
        <button v-on:click="hello">click me</button>

        <br>
        <br>
        <hr>
        <br>    
    </div>
</template>

<script>
export default {
    name: "ternoryOperator",
    data() {
        return {
            myData: {
                name: "samir",
                age: 24,
                ok: true
            }
        }
    },
    methods: {
        hello() {
            this.myData.ok = !this.myData.ok
        }
    }

}
</script>

<!-- 
------- Understanding the Code:---------

The code you provided is a Vue.js component. It consists of a template section and a script section. The template
section defines the HTML structure of the component, while the script section contains the JavaScript logic.

In the template section, there is an h3 element that displays the value of the ok property using a ternary operator. If
ok is true, it displays "yes"; otherwise, it displays "no". There is also a button with a click event listener that
calls the hello method when clicked.

In the script section, the component is defined with the name "ternaryOperator". It has a data function that returns an
object with a property called myData. myData contains a name property set to "samir", an age property set to 24, and an
ok property set to true. The component also has a methods object that contains a hello method. The hello method toggles
the value of the ok property by negating its current value. -->