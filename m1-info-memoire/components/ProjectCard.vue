<template>
  <div
    class="flex flex-col gap-1 border border-1 rounded p-4 w-96 h-fit justify-between bg-gray-100/50 overflow-clip"
  >
    <div class="flex flex-col gap-1 relative">
      <div
        class="absolute -top-5 -right-7 text-6xl -rotate-20 animate-pulse duration-700"
      >
        <slot name="icon" />
      </div>
      <span class="text-xl font-semibold">
        <slot name="title" />
      </span>
      <div class="flex gap-2 mb-4">
        <slot name="tags" />
      </div>
    </div>
    <span class="text-sm opacity-70"> <slot name="description" /> </span>
  </div>
</template>
