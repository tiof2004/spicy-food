<template>
  <div>
    <div class="bg-[#fffeff] shadow-2xl py-4 rounded-md">
      <div class="flex justify-between items-center px-4 xl:my-4">
        <h1
          class="bg-[#efefef] h-10 w-10 rounded-full hover:bg-[#1fa15c] flex items-center justify-center"
        >
          <img :src="pop1" alt="" class="w-4" />
        </h1>
        <h1
          class="bg-[#efefef] h-10 w-10 rounded-full flex items-center justify-center hover:bg-[#1fa15c]"
        >
          <img :src="pop2" alt="" class="w-5" />
        </h1>
      </div>
      <div class="flex justify-center items-center">
        <div class="flex flex-col justify-center items-center">
          <img :src="pop3" alt="" />
          <p class="text-gray-700 text-xl">{{ pop4 }}</p>
          <p>{{ pop5 }}</p>
          <span class="flex items-center space-x-3 hover:text-lg">
            <p class="text-xl text-[#1fa15c]">{{ pop6 }}</p>
            <button
              class="bg-[#182b56] text-white px-6 py-1 rounded-md hover:bg-[#1fa15c]"
            >
              <p>{{ pop7 }}</p>
            </button>
          </span>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'PopularComponents',
  props: {
    pop1: {
      type: String,
      default: ''
    },
    pop2: {
      type: String,
      default: ''
    },
    pop3: {
      type: String,
      default: ''
    },
    pop4: {
      type: String,
      default: ''
    },

    pop5: {
      type: String,
      default: ''
    },
    pop6: {
      type: String,
      default: ''
    },
    pop7: {
      type: String,
      default: ''
    }
  }
}
</script>
