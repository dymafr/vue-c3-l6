<template>
  <h1 @click="userClick()">Bonjour tout le monde !</h1>
  <input type="text" @input="userInput()" />
</template>

<script setup lang="ts">
function userClick(event: MouseEvent) {
  console.log(event);
}

function userInput(input: string, event: Event) {
  const target = event.target as HTMLInputElement;
  target.value = 'Bonjour';
  console.log(input);
}
</script>

<style></style>
