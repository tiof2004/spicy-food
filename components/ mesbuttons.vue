<template>
  <div>
    <div class="space-x-4 flex">
      <button
        class="bg-green-600 h-8 w-8 rounded-full xl:hidden flex justify-center items-center"
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
</template>
<script>
export default {
  name: 'MesbuttonsComponets',
  data() {
    return {
      printserche: false,
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
    }
  }
}
</script>
