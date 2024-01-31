<script setup lang="ts">
const handleClick = () => {
  console.log('Click');
};
</script>
<template>
  <section>
    <div>こんにちは</div>
    <UButton @click="handleClick">ボタン</UButton>
    <Sample />
  </section>
</template>
