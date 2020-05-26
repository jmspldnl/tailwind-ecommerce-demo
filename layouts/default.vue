<template>
  <div class="flex flex-col min-h-screen">
    <header>
      <div class="bg-red-600 py-2">
        <div class="container mx-auto text-center text-white">DEMO STORE</div>
      </div>
      <div class="container flex mx-auto">
        <nuxt-link
          class="p-4 text-5xl"
          :class="{ test: test }"
          to="/"
          @mouseover="test = true"
          @mouseleave="test = false"
          >Shop</nuxt-link
        >
      </div>
      <div class="bg-blue-500">
        <nav
          class="container mx-auto flex items-center justify-between flex-wrap"
        >
          <div class="block lg:hidden">
            <button
              class="flex items-center px-3 py-2 border rounded text-teal-200 border-teal-400 hover:text-white hover:border-white"
            >
              <svg
                class="fill-current h-3 w-3"
                viewBox="0 0 20 20"
                xmlns="http://www.w3.org/2000/svg"
              >
                <title>Menu</title>
                <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
              </svg>
            </button>
          </div>
          <div
            class="w-full block flex-grow hidden lg:flex lg:items-center lg:w-auto"
          >
            <ul class="text-sm lg:flex-grow flex">
              <li
                v-for="(item, i) in items"
                :key="i"
                class="relative"
                @mouseover="item.active = true"
                @mouseleave="item.active = false"
              >
                <nuxt-link
                  :to="item.to"
                  class="block p-4 lg:inline-block lg:mt-0 text-blue-100 hover:bg-blue-400 hover:text-white transition-colors duration-300"
                >
                  {{ item.title }}
                </nuxt-link>
                <ul
                  v-if="item.items"
                  :class="{ flex: item.active, hidden: !item.active }"
                  class="absolute top-100 flex-col flex-wrap"
                >
                  <li v-for="(child, j) in item.items" :key="j">
                    <nuxt-link
                      :to="child.to"
                      class="block p-4 lg:inline-block lg:mt-0 bg-blue-500 text-blue-100 hover:bg-blue-400 hover:text-white relative transition-colors duration-300"
                    >
                      {{ child.title }}
                    </nuxt-link>
                  </li>
                </ul>
              </li>
            </ul>
          </div>
        </nav>
      </div>
    </header>
    <div class="container mx-auto">
      <nuxt />
    </div>
    <footer class="bg-gray-300 mt-auto">
      <div class="container mx-auto px-4 py-4">
        <div class="flex flex-wrap -mx-4">
          <div
            v-for="i in 3"
            :key="i"
            class="my-4 px-4 w-full md:w-1/2 xl:w-1/4"
          >
            <h6 class="text-lg text-gray-800 font-bold uppercase mb-4">
              Heading
            </h6>
            <ul>
              <li v-for="j in 4" :key="j">
                <n-link
                  class="inline-block text-gray-700 hover:text-black transition-colors duration-300 py-1 hover:underline"
                  to="/"
                  >Link {{ j }}</n-link
                >
              </li>
            </ul>
          </div>
          <div class="my-4 px-4 w-full md:w-1/2 xl:w-1/4">
            <h6 class="text-lg text-gray-800 font-bold uppercase mb-4">
              Newsletter Signup
            </h6>
            <form
              class="border border-gray-400 rounded flex flex-no-wrap overflow-hidden"
            >
              <input
                class="bg-white focus:outline-none focus:shadow-outline py-2 px-4 block w-full appearance-none leading-normal"
                type="email"
                placeholder="jane@example.com"
              />
              <button
                class="bg-gray-300 hover:bg-gray-200 border-l border-gray-400 transition-colors duration-300 px-3 whitespace-no-wrap text-sm font-bold uppercase text-gray-600"
              >
                Sign Up
              </button>
            </form>
          </div>
        </div>
      </div>
      <div class="bg-gray-800 text-white">
        <div class="container mx-auto p-4 text-center">
          Copyright &#169; {{ new Date().getFullYear() }} Demo Store LLC. All
          Rights Reserved.
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      test: false,
      items: []
    }
  },
  created() {
    for (let i = 1; i <= 8; i++) {
      const item = {
        title: 'Category ' + i,
        active: false,
        to: { name: 'category' }
      }
      item.items = []
      for (let j = 1; j <= 5; j++) {
        item.items.push({
          title: 'Category ' + j,
          to: { name: 'category' }
        })
      }
      this.items.push(item)
    }
  }
}
</script>
