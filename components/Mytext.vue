<template>
  <div>
    <div>
      <div v-if="textStyle === 'TITLE'">
        <h1 class="xl:text-2xl text-xl text-gray-400 font-bold">
          {{ myText }}
        </h1>
      </div>
      <div v-if="textStyle === 'SOUPTITLE'">
        <h1 class="text-6xl font-bold">
          {{ myText }}
        </h1>
      </div>
      <div v-if="textStyle === 'SOUPETITLE'">
        <h1 class="xl:text-4xl text-3xl text-gray-400 font-bold">
          {{ myText }}
        </h1>
      </div>
      <div v-if="textStyle === 'SOUPITITLE'">
        <h1>
          {{ myText }}
        </h1>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'MytextComponents',
  props: {
    myText: {
      type: String,
      default: ''
    },
    textStyle: {
      type: String,
      default: ''
    }
  }
}
</script>
