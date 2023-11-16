<template>
  <div class="xl:px-24 px-6">
    <div class="flex justify-center items-center py-6">
      <div class="text-center">
        <p class="text-[#1fa15c] text-xl">Our Dish</p>
        <h1 class="text-[#182b56] font-bold text-2xl">POPULAR DISHES</h1>
      </div>
    </div>
    <div
      class="xl:grid xl:grid-cols-3 gap-4 space-y-3 justify-center items-center"
    >
      <popular
        v-for="(item, index) in popular"
        :key="index"
        :pop1="item.pop1"
        :pop2="item.pop2"
        :pop3="item.pop3"
        :pop4="item.pop4"
        :pop5="item.pop5"
        :pop6="item.pop6"
        :pop7="item.pop7"
      />
    </div>
  </div>
</template>
<script>
export default {
  name: 'SouspopularComponents',
  data() {
    return {
      popular: [
        {
          pop1: require('../assets/images/sms.png'),
          pop2: require('../assets/images/javascript.png'),
          pop3: require('../assets/images/hamber.jpeg'),
          pop4: 'Tasty Food',
          pop5: 'star',
          pop6: '$15.99',
          pop7: 'Add To Cart'
        },
        {
          pop1: require('../assets/images/sms.png'),
          pop2: require('../assets/images/javascript.png'),
          pop3: require('../assets/images/gateau.png'),
          pop4: 'Tasty Food',
          pop5: 'star',
          pop6: '$15.99',
          pop7: 'Add To Cart'
        },
        {
          pop1: require('../assets/images/sms.png'),
          pop2: require('../assets/images/javascript.png'),
          pop3: require('../assets/images/poulet.jpeg'),
          pop4: 'Tasty Food',
          pop5: 'star',
          pop6: '$15.99',
          pop7: 'Add To Cart'
        },
        {
          pop1: require('../assets/images/sms.png'),
          pop2: require('../assets/images/javascript.png'),
          pop3: require('../assets/images/plat.jpeg'),
          pop4: 'Tasty Food',
          pop5: 'star',
          pop6: '$15.99',
          pop7: 'Add To Cart'
        },
        {
          pop1: require('../assets/images/sms.png'),
          pop2: require('../assets/images/javascript.png'),
          pop3: require('../assets/images/chocola.jpeg'),
          pop4: 'Tasty Food',
          pop5: 'star',
          pop6: '$15.99',
          pop7: 'Add To Cart'
        },
        {
          pop1: require('../assets/images/sms.png'),
          pop2: require('../assets/images/javascript.png'),
          pop3: require('../assets/images/coul.png'),
          pop4: 'Tasty Food',
          pop5: 'star',
          pop6: '$15.99',
          pop7: 'Add To Cart'
        }
      ]
    }
  }
}
</script>
