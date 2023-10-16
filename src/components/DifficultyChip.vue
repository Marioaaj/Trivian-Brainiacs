<script setup>
const props = defineProps({
  difficulty: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <p
    class="difficulty"
    :class="
      props.difficulty === 'easy'
        ? 'bg-slate-950'
        : props.difficulty === 'medium'
        ? 'bg-slate-950'
        : 'bg-slate-950'
    "
  >
    {{ props.difficulty }}
  </p>
</template>

<style lang="postcss" scoped>
.difficulty {
  @apply absolute bottom-6 left-8 rounded-full px-4 py-2 font-bold capitalize text-slate-700 text-white;
}
</style>
