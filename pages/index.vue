<template>
  <div class="my-4">
    <client-only>
      <carousel v-bind="options">
        <slide v-for="i in 12" :key="i">
          <product class="w-full">
            <div>Product {{ i }}</div>
            <div>$9.99</div>
          </product>
        </slide>
      </carousel>
    </client-only>
    <div class="flex flex-wrap">
      <product
        v-for="i in 12"
        :key="i"
        class="w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/6"
      >
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
        perPage: 1,
        perPageCustom: [
          [768, 2],
          [1024, 3],
          [1280, 4]
        ],
        paginationEnabled: false,
        navigationEnabled: true
      }
    }
  }
}
</script>
