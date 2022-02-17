<template></template>

<script setup lang="ts">
interface User {
  name: string;
  age: number | string;
}

let user: User | null;

function createUser(name: string): User | null {
  return {
    name,
    age: 18,
  };
}

user = createUser('Paul');
</script>

<style></style>
