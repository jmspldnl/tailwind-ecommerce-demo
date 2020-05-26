<template>
  <div class="my-4">
    <client-only>
      <carousel v-bind="options">
        <slide v-for="i in 8" :key="i">
          <product class="w-full">
            <div>Product {{ i }}</div>
            <div>$9.99</div>
          </product>
        </slide>
      </carousel>
    </client-only>
    <div class="flex flex-wrap">
      <product v-for="i in 12" :key="i" class="w-1/6">
        <div>Product {{ i }}</div>
        <div>$9.99</div>
      </product>
    </div>
  </div>
</template>

<script>
import product from '~/components/product.vue'

export default {
  components: {
    product
  },
  data() {
    return {
      options: {
        loop: true,
        perPageCustom: [
          [768, 3],
          [1024, 4]
        ],
        paginationEnabled: false,
        navigationEnabled: true
      }
    }
  }
}
</script>
