<script setup lang="ts">

import type { NavigationMenuItem } from '@nuxt/ui'

const items = ref<NavigationMenuItem[][]>([
  [
    {
      label: 'layout',
      icon: 'i-lucide-box',
      active: true,
      defaultOpen: true,
      children: [
        {
          label: 'aspect-ratio',
          icon: 'i-lucide-file-text',
          to: '/page1'
        },
        {
          label: 'columns',
          icon: 'i-lucide-file-text',
          to: '/page2'
        },
        {
          label: 'break-after',
          icon: 'i-lucide-file-text',
          to: '/page3'
        },
        {
          label: 'break-before',
          icon: 'i-lucide-file-text',
          to: '/page4'
        },
        {
          label: 'break-inside',
          icon: 'i-lucide-file-text',
          to: '/page5'
        },
        {
          label: 'box-decoration-break',
          icon: 'i-lucide-file-text',
          to: '/page6'
        },
        {
          label: 'box-sizing',
          icon: 'i-lucide-file-text',
          to: '/page7'
        },
        {
          label: 'display',
          icon: 'i-lucide-file-text',
          to: '/page8'
        },
        {
          label: 'float',
          icon: 'i-lucide-file-text',
          to: '/page9'
        },
        {
          label: 'object-fit',
          icon: 'i-lucide-file-text',
          to: '/page10'
        },
        {
          label: 'object-position',
          icon: 'i-lucide-file-text',
          to: '/page11'
        },
        {
          label: 'overflow',
          icon: 'i-lucide-file-text',
          to: '/page12'
        },
        {
          label: 'object-fit',
          icon: 'i-lucide-file-text',
          to: '/page13'
        },
        {
          label: 'position',
          icon: 'i-lucide-file-text',
          to: '/page14'
        },
        {
          label: 'visibility',
          icon: 'i-lucide-file-text',
          to: '/page15'
        },
        {
          label: 'z-index',
          icon: 'i-lucide-file-text',
          to: '/page16'
        },
      ]
    },
    {
      label: 'grid / flexbox',
      icon: 'i-lucide-box',
      active: true,
      defaultOpen: true,
      children: [
        {
          label: 'flex-basis',
          icon: 'i-lucide-file-text',
          to: '/page17'
        },
        {
          label: 'flex-col',
          icon: 'i-lucide-file-text',
          to: '/page18'
        },
      ]
   }
    

  ],
  [
    {
      class:'justify-center',
      label: 'GitHub',
      icon: 'i-simple-icons-github',
      to: 'https://github.com/Efril1',
      target: '_blank'
    }
  ]
])
</script>

<template>
    <div class="flex min-h-screen">
      <div class="w-48 fixed">
        <UNavigationMenu
          orientation="vertical"
          :items="items"
        />
      </div>
      
      <main class="ml-48 flex-1 p-4">
        <div>
          <slot />
        </div>
      </main>
    </div>
  </template>