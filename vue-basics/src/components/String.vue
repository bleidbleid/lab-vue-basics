<template>
    <div class="section">
        <button @click="cool = !cool">Cançó!</button>
        <h1 v-if="cool">Un, dos, tres,
Som tres bessones,
Us durem sols una estona,
Viatjant al cor dels contes.
Tres ratolins són els nostres veïns.
Malgrat que fem trapelleries,
Sempre sabem quan ja n'hi ha prou,
I si la bruixa ens castiga,
T'explicarem un conte nou.
Un, dos, tres,
Moltes vegades,
Coneixem serps encantades,
Llops i nans, ogres i fades,
I un mussol que mai no saps què vol.
Un, dos, tres
Vindrà la bruixa.
Un, dos, tres,
Si la dibuixes.
Un, dos tres,
Li farem bromes.
Un, dos, tres,
Les tres bessones.
Un, dos, tres!</h1>
    </div>
</template>

<script setup>
import { ref } from 'vue';
const cool = ref(false);

// function string() {
//cool.value = !cool.value;
// }
</script>
<style scoped>
h1 {
    font-size: 24px;
}
button {
    font-family: 'Patrick Hand SC', cursive;
    font-size: 2rem;
    padding: 4px 16px;
    color: #F3EAE5;
    background-color: #A56DA6;
}

button:hover {
    color: #A56DA6;
    background-color: #F3EAE5;
    border-color: #A56DA6;
}
</style>