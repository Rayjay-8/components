<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from './components/HelloWorld.vue'
import LabelTag from './components/LabelTag.vue'
import ToggleSwitch from './components/ToggleSwitch.vue'
import Usandolots from './components/Usandoslots.vue'


</script>

<template>

  <!-- <Usandolots title="Tab 1"> exemplo 1</Usandolots>
  <Usandolots title="Tab 2"> exemplo 2</Usandolots>
  <Usandolots title="Tab 3"> exemplo 3</Usandolots> -->

  <h1>{{items}}</h1>

  <LabelTag></LabelTag>

</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
      display: grid;
    align-content: center;
    justify-content: center;
    align-items: center;
    justify-items: center;

}
</style>
