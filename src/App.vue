<template>
  <div>
    <p>{{ message }}</p>
    <button @click="changeMessage">change</button>
  </div>
</template>

<script>
import { ref } from 'vue'
  
  export default {
    // data() {
    //   return {
    //     message: 'hello'
    //   }
    // },
    // methods: {
    //   changeMessage() {
    //     this.message = 'hi'
    //   }
    // }
    setup() {
      const message = ref('hello');

      function changeMessage() {
        message.value = 'hi';
      }

      return { message, changeMessage }
    }
  }
</script>

<style lang="scss" scoped>

</style>