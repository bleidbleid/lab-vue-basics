<template>
    <div class="card">
        <div class="card-image">
            <figure class="image is-4by3">
                <img :src="props.image" alt="Placeholder image">
            </figure>
        </div>
        <!-- :class="colorCard ? 'color4' : 'coloret5'"  -->
        <div class="card-content" :style="colorCard ? { 'background-image': 'linear-gradient(213deg, #FB708D 0%, 1.1627906933426857%, #FC6FBE 2.3255813866853714%, 9.302325733006%, #FA9776 16.27907007932663%, 23.9534892141819%, #FBE182 31.62790834903717%, 34.8837211728096%, #E5FD81 38.13953399658203%, 44.186046719551086%, #BDFC89 50.23255944252014%, 54.883721470832825%, #92FDB5 59.53488349914551%, 65.11628031730652%, #94FCE3 70.69767713546753%, 74.88372325897217%, #9DEAFA 79.0697693824768%, 88.13953697681427%, #A1C4FC 97.20930457115173%, 98.60465228557587%, #B5A5FE 100%)'} :{ 'background-color': props.activeColor}">
            <div class="content" >
                <div class="card-title">{{props.title}}</div>
                <div>{{props.description}}</div>
            </div>
            <button @click="colorCard = !colorCard">Color!</button>
        </div>
    </div>
</template>
<script setup>
import { ref } from 'vue'
import { defineProps } from 'vue'
// Definimos los props que vamos a recibir en el componente
const props = defineProps(['title', 'description', 'image', 'activeColor']);
const colorCard = ref(true);

</script>
<style scoped>
.card{
    display: flex;
    flex-direction: column;
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
    font-size: 2rem;
}

button {
    font-family: 'Patrick Hand SC', cursive;
    font-size: 1.2rem;
    padding: 4px 16px;
    color: #A56DA6;
    background-color: #F3EAE5;
    border-color: #A56DA6;
}

button:hover {
    color: #F3EAE5;
    background-color: #A56DA6;
}
</style>