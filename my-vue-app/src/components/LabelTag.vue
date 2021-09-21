<script setup>
import { ref, computed } from 'vue'

let opcselect = ref('opt3')
//opção selecionada padrão
//var opcselect = "rayyy"


</script>

<template>
    <div class="label">
        
        <p @click="opcselect = 'opt1'" :class="{ 'pSelect': opcselect == 'opt1' }">opt1</p>
        <p @click="opcselect = 'opt2'" :class="{ 'pSelect': opcselect == 'opt2' }">opt2</p>
        <p @click="opcselect = 'opt3'" :class="{ 'pSelect': opcselect == 'opt3' }">opt3</p>
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
    cursor: pointer;
}
p:hover{
    background-color: rgb(229, 216, 245);
}
.pSelect{
    
    background-color: #242350;
}
.pSelect:hover{
    background-color:#242350!important;
}
</style>
