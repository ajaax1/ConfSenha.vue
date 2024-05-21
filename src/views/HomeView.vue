<script setup>
import { ref } from 'vue';
let senha = ref('');
let confirmar = ref('');

</script>

<template>
  <main class="flex justify-center items-center h-screen bg-orange-100	">
    <form action="" class="flex flex-col gap-2 bg-stone-200 border shadow-lg p-4">
      <input class="border border-black" placeholder=" email"  type="text">
      <input class="border border-black" placeholder=" senha"  type="text" v-model="senha">
      <input class="border border-black" placeholder=" confirmar"  type="text" v-model="confirmar">
      <small v-show="senha != confirmar" class="text-red-600">A senha não corresponde</small>
      <button class="border bg-white  border-black">Login</button>
    </form>
  </main>
</template>
