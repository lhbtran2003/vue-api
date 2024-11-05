<script setup lang="ts">
import axios from "axios";
import {createLogger} from "vite";

const getAllProducts = async () => {
  const res = await axios.get("http://localhost:3001/post");
  return res.data;
}

// console.log(getAllProducts().then(res => res.data));
getAllProducts().then(res =>  console.log(res));
</script>

<template>

</template>

<style scoped>

</style>