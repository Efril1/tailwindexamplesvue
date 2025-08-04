<template>
    <div class="h-40 w-40 overscroll-none overflow-scroll border p-4 rounded">
      <div v-for="i in 20" :key="i" class="py-2">
        <UAvatar src="https://avatars.githubusercontent.com/u/739984?v=4" size="xs" />
        <span class="ml-2">Item {{ i }}</span>
      </div>
    </div>
  </template>