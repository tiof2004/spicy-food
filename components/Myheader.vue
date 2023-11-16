<template>
  <div>
    <div class="shadow-2xl shadow-[#dad7d7] bg-[#fffeff]">
      <div class="flex justify-between items-center xl:px-24 px-8 py-4">
        <div>
          <h1 class="text-xl font-bold text-[#182b56]">Logo</h1>
        </div>
        <div
          class="xl:flex hidden items-center justify-center space-x-8 text-gray-400"
        >
          <div v-for="(item, index) in navs" :key="index">{{ item.name }}</div>
        </div>

        <div class="space-x-4 flex">
          <button
            class="bg-green-600 h-8 w-8 rounded-full xl:hidden flex justify-center items-center"
            @click="menuebut"
          >
            <img src="../assets/images/menu.png" alt="" class="w-5" />
          </button>
          <button
            class="w-45 bg-[#efefef] h-8 w-8 rounded-full flex items-center justify-center"
            @click="serch"
          >
            <img src="../assets/images/search.png" alt="" class="w-5" />
          </button>
          <button
            class="w-45 bg-[#efefef] h-8 w-8 rounded-full flex items-center justify-center"
          >
            <img src="../assets/images/coeur.jpeg" alt="" class="w-5" />
          </button>
          <button
            class="w-45 bg-[#efefef] h-8 w-8 rounded-full flex items-center justify-center"
          >
            <img src="../assets/images/bourwet.png" alt="" class="w-5" />
          </button>
        </div>
      </div>
    </div>

    <div
      :class="`${
        printmenue === false ? 'hidden' : ''
      } w-full bg-slate-200 top-0 text-center justify-center items-center py-4 h-screen `"
    >
      <div class="space-y-4">
        <div v-for="(item, index) in navs" :key="index">
          <p>{{ item.name }}</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'MyheaderComponents',
  data() {
    return {
      printserche: false,
      printmenue: false,
      navs: [
        {
          path: '#home',
          name: 'Home'
        },
        {
          path: '#dishes',
          name: 'Dishes'
        },
        {
          path: '#about',
          name: 'About'
        },
        {
          path: '#menu',
          name: 'Menu'
        },
        {
          path: '#reviw',
          name: 'Reviw'
        },
        {
          path: '#order',
          name: 'Order'
        }
      ]
    }
  },
  head: {
    title: 'mamat'
  },
  methods: {
    cross() {
      this.printnav = false
    },
    menu() {
      this.printnav = true
    },
    serch() {
      this.printserche = true
    },
    butserch() {
      this.printserche = false
    },
    menuebut() {
      this.printmenue = !this.printmenue
    }
  }
}
</script>
