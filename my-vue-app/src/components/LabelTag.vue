<script setup>
import { ref, computed } from 'vue'

//const selecionado = ref(false)
//opção selecionada padrão
var opcselect = ref('opt2')


function select(value){
    console.log("---------")

    console.log(opcselect.value)
    opcselect = ref(opcselect.value)
    const twiceTheCounter = computed(() => opcselect = value)

    console.log(opcselect.value)
}
</script>

<template>
    <div class="label">
        
        <p @click="select('opt1')" :class="{ 'pSelect': opcselect == 'opt1' }">opt1</p>
        <p @click="select('opt2')" :class="{ 'pSelect': opcselect == 'opt2' }">opt2</p>
        <p @click="select('opt3')" :class="{ 'pSelect': opcselect == 'opt3' }">opt3</p>
    </div>

    <h1>opcao selecionada {{opcselect}}</h1>
</template>

<style scoped>
.label {
    display: flex;
    width: fit-content;
    color: #42b983;
    border: 2px solid #222;
    border-radius: 8px;
}

p{
    margin: 2px;
    padding: 8px;
    background-color: rgb(255, 255, 255);
    border-radius: 8px;
}
.pSelect{
    
    background-color: #242350;
}
</style>
