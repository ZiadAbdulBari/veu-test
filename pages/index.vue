<template>
<div>
  <Introduction/>
  <LargeCard 
    v-for="largeCard in largeCardInfo" 
    :key="largeCard.id" 
    :largeCardData="largeCard"
  />

  <SmallCard
    v-for="smallCard in smallCardInfo" 
    :key="smallCard.id" 
    :smallCardData="smallCard"
  />
</div>
</template>

<script>
import Introduction from '~/components/Introduction.vue'
import LargeCard from '~/components/LargeCard.vue'
import SmallCard from '~/components/SmallCard.vue'
import {largeCardSections,smallCardSections} from '~/assets/data.js'
export default {
  data(){
    return{
      largeCardInfo:largeCardSections,
      smallCardInfo:smallCardSections
    }
  }
}
// console.log(largeCardSections)
</script>

Introduction