
<template>
<p>{{ contador }}</p>
<button @click="incrementar">Incrementar</button>
<button @click="decrementar">Decrementar</button>

</template>

<script setup>
// esta parte hara uso del parametro de reactividad de vue3, usando objetos reactivos como "ref"
//importamos ref, para crear una referencia reactiva al valor
import{ref} from 'vue';
const contador= ref(0);
const incrementar = ()=>{
    contador.value++;
}
const decrementar = ()=>{
    contador.value--;
}
</script>

<style scoped>
p {
    color:red;
}
</style>
