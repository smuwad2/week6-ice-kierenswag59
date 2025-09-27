<script>
    export default { 
        // Add Code Here
        // challenge: use array  
        data() {
            return {
                fruit1: 'cake',
                fruit2: 'pineapple',
                fruit3: 'dinosaur',
                fruits: ["cake","pineapple","dinosaur"]
            }
        },
    }
</script>

<template>
    <div id="app">
        {{ message }} </br>
        {{ fruit1 }} <input type="radio" name="fruit">
        {{ fruit2 }} <input type="radio" name="fruit">
        {{ fruit3 }} <input type="radio" name="fruit">
        <br>
        <span v-for="fruit in fruits">

            {{ fruit }} <input type="radio" name="fruit">
        </span>
    </div>
</template>


<style scoped>
</style>
