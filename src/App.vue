<template>
  <div>
    <flipbook class="flipbook" :pages="['array', 'of', 'image', 'URLs']" v-slot="flipbook">
      <button @click="flipbook.flipLeft">Previous Page</button>
      <button @click="flipbook.flipRight">Next Page</button>
    </flipbook>
  </div>
</template>

<script>
import Flipbook from 'flipbook-vue';

export default {
  components: { Flipbook },
};
</script>

<style>
.flipbook {
  
  width: 90vw;
  height: 90vh;
}
</style>

