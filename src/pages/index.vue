<!-- eslint-disable vue/singleline-html-element-content-newline -->
<template>
  <div h-full bg="#edeff1" text-center flex="~" justify-center items-center>
    <div>
      <div>{{ store.num }}</div>
      <button red-btn @click="store.num++">+</button>
    </div>
  </div>
</template>

<script setup lang="ts">
import { useStore } from '@/store/user'

const store = useStore()
</script>

<style>
  .after {
    content: "";
    display: block;
    width: 120px;
    height: 20px;
  }
</style>
