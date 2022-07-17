<template>
  <div>
    <h3>Password hide/show System</h3>
    <g-input />
    <br>
  </div>
</template>

<script>
import GInput from './GInput.vue'

export default {
  name: 'GComponent',
  components: {
    GInput
  },
  props: {
    style: {
      type: String,
    }
    },
}
</script>

<style scoped>
h3 {
  margin: 40px 20 0;
  color: rgb(136, 136, 250);
}
</style>
