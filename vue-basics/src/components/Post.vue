<template>
    <div class="card">
        <div class="card-image">
            <figure class="image is-4by3">
                <img :src="props.image" alt="Placeholder image">
            </figure>
        </div>
        <div class="card-content"  :class="colorCard ? 'color4' : 'coloret2'" >
            <div class="content">
                <div class="card-title">{{props.title}}</div>
                <div>{{props.body}}</div>
                <h1>{{props.index}}</h1>
            </div>
            <button class="button" @click="colorCard = !colorCard">Color!</button>
        </div>
    </div>
</template>
<script setup>
import { ref } from 'vue'
import { defineProps } from 'vue'
// Definimos los props que vamos a recibir en el componente
const props = defineProps(['title', 'body', 'image']);
const colorCard = ref(true);

</script>
<style scoped>
.card{
    display: flex;
    flex-direction: column;
}

.color4 {
    background-color: white;
} .coloret0 {
    background-color: yellowgreen;
} 

.coloret1 {
    background-color: blue;
} 

.coloret2 {
    background-color: violet;
} 
.card-content{
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: flex-start;
}
.card-title{
    font-weight: bold;
    font-size: 1.2rem;
}
</style>