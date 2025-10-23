<script>
    export default { 
        // Add code in appropriate places
        data() {
            return {
                items: ['keyboard', 'mouse', 'iPhone', 'macbook', 'adapter']
            }
            
        }
    }
</script>

<template>

    <h2>Shopping Cart</h2>
    <!-- TODO: Add Code Here -->
    <ul v-for="item in items">
        <li>{{ item }} <button @click="items.splice(items.indexOf(item), 1)">Delete</button></li>
    </ul>


    <input v-model="addItem" /> <button @click="items.push(addItem)">Add!</button>
   
</template>
