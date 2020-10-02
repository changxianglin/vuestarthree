<template>
  <h1>{{ msg }}</h1>
  <button @click="data.count++">count is: {{ data.count }}</button>
  <p>Edit <code>components/HelloWorld.vue</code> to test hot module replacement.</p>
</template>

<script>
import { reactive } from 'vue'
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  setup() {
    const data = reactive({
      count: 1,
    })

    return {data}
  }
}
</script>
