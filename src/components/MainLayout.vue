<script setup>
import MainScore from '@/components/MainScore.vue'
</script>

<template>
  <main>
    <div class="card">
      <RouterView />      
    </div>
  </main>
  <MainScore />
</template>

<style lang="postcss" scoped>
main {
  @apply flex h-screen items-center justify-center bg-gradient-to-bl from-yellow-200 via-pink-200 to-pink-400;

  & .card {
    @apply flex h-5/6 min-h-fit w-11/12 flex-col items-center gap-16 overflow-auto rounded-lg bg-white p-8 shadow-lg;
  }
}

.score {
  @apply absolute bottom-6 right-8 text-2xl font-bold uppercase text-slate-700;
}
</style>