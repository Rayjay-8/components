<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from './components/HelloWorld.vue'
import LabelTag from './components/LabelTag.vue'
import ToggleSwitch from './components/ToggleSwitch.vue'
import Usandolots from './components/Usandoslots.vue'



</script>

<template>
  <LabelTag @erro-grave-004="triggerToast" />
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {
    const showToast = ref(false)
    const triggerToast = () => {
      showToast.value = true;
      setTimeout(() => showToast.value = false, 3000)
    }
    return { showToast, triggerToast }
  }
}
</script>

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
