<script setup lang="ts">
import { useCounterStore } from '@/store/counterStore';

const counterStore = useCounterStore();

const { count: countState } = storeToRefs(counterStore);
const { increment } = counterStore;
</script>
<template>
  <section>
    <div>こんにちは</div>
    <UButton @click="increment">ボタン</UButton>
    <Sample :count="countState" />
  </section>
</template>
