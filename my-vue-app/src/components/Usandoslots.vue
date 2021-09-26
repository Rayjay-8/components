<template>
  <div>
      {{ tabTitles }}
      <slot/>
  </div>

</template>

<script >
import { ref} from 'vue'

export default {
    setup (props, { slots }) {
        const tabTitles = ref(slots.default().map((tab) => tab.props.title))
        return {
            tabTitles,
        }
    },
    
}

</script>

<style>

</style>