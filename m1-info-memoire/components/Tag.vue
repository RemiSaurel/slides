<script setup lang="ts">
defineProps<{ content: string }>();

const bgColor = {
  Design: "bg-red-400",
  Dev: "bg-blue-400",
  IA: "bg-green-400",
  Archi: "bg-yellow-400",
  Mobile: "bg-purple-400",
};

const borderColor = {
  Design: "border-red-200",
  Dev: "border-blue-200",
  IA: "border-green-200",
  Archi: "border-yellow-300",
  Mobile: "border-purple-200",
};
</script>

<template>
  <div
    class="rounded-lg text-xs border border-1 px-2 py-0.5 bg-white flex items-center gap-2"
    :class="`${borderColor[content]}`"
  >
    <span class="w-2 h-2 rounded-full" :class="`${bgColor[content]}`"></span>
    {{ content }}
  </div>
</template>
