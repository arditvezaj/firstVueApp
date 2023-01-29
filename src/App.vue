<script setup>
import { ref } from 'vue';

const count = ref(0);
</script>

<template>
  <body>
    <div class="count">
      <h1>Your count is...</h1>
      <input type="number" :value="`${count}`"/>
      <div>
        <button @click="count--">-</button>
        <button @click="count++">+</button>
      </div>
    </div>
  </body>
</template>

<style scoped>
body {
  background-color: rgb(97, 211, 152);
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.count {
 
  width: 100%;
  margin: 0 auto;
}

h1 {
  font-size: 70px;
  margin-bottom: 30px;
}

input {
  font-size: 30px;
  text-align: center;
}

button {
  width: 50px;
  height: 50px;
  font-size: 40px;
  margin: 25px 4px
}
</style>
