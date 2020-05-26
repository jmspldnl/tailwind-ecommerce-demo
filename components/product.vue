<template>
  <nuxt-link
    to="/product"
    class="flex flex-col box-border p-4 w-1/4 hover:shadow transition-shadow"
  >
    <div class="bg-gray-100 relative" style="padding-bottom:100%">
      <img class="absolute inset-0 h-full w-full object-cover" />
    </div>
    <div class="my-2">
      <slot></slot>
    </div>
  </nuxt-link>
</template>
