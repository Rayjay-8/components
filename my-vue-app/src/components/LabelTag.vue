<script setup>
import { ref } from 'vue'



const items = [
        {'message':'Label-1'},
        {'message':'Label-2'},
        {'message':'Label-3'},
        {'message':'Label-4'}
    ]

let ValorPadrao = 'Label-2'
let opcselect = ref(ValorPadrao)

</script>



<template>
    
    <div class="label" >
      
    
        <div v-for="item in items" :key="item.message">
            <p @click="opcselect = item.message" :class="{ 'pSelect': opcselect == item.message }">{{item.message}}</p>
        </div>
    </div>

    <h1>opcao selecionada {{opcselect}}</h1>
</template>

<style scoped>
.label {
    display: flex;
    width: fit-content;
    color: #000000;
    border: 1.5px solid #9e9e9e;
    border-radius: 8px;
}

p{
    margin: 3px;
    padding: 8px;
    background-color: rgb(255, 255, 255);
    border-radius: 0.3rem;
    color: #9e9e9e;
    cursor: pointer;
}
p:hover{
    background-color: #ececec30;
}
.pSelect{
    
    background-color: #464656;
    color: aliceblue;
}
.pSelect:hover{
    background-color:#464656!important;
}
</style>
