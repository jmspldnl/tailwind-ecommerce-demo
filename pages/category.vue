<template>
  <div class="flex flex-col lg:flex-row my-4">
    <div class="p-4 w-full lg:w-1/5">
      <h2 class="text-2xl">Refine By</h2>
    </div>
    <div class="p-4 w-full lg:w-4/5">
      <h2 class="text-2xl">Category</h2>
      <div class="flex flex-wrap -mx-4 my-4">
        <product v-for="i in 24" :key="i" class="w-1/2 md:w-1/3 lg:w-1/4">
          <div>Product {{ i }}</div>
          <div>$9.99</div>
        </product>
      </div>
    </div>
  </div>
</template>

<script>
import product from '~/components/product.vue'
export default {
  components: {
    product
  }
}
</script>
