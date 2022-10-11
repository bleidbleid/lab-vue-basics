<template>
    <div>
        <h1>{{2+2}}</h1>
        <button @click="cool = !cool">Surprise!</button>
        <h1 v-if="cool">This is a cool string!</h1>
    </div>
</template>

<script setup>
import { ref } from 'vue';
const cool = ref(false);

// function string() {

//      cool.value = !cool.value;
// ;

// }
</script>

<style scoped>

</style>