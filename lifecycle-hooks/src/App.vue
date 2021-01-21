<template>
  <div>
    <h1>Life Cycle Hooks</h1>
  </div>
</template>

<script>
import { onMounted } from 'vue'

export default {
  setup() {
    onMounted(() => {
      console.log('Foi montado com composition API')
    })
  }
}
</script>