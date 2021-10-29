<template>
<div>
  <Navbar/>
  <Introduction/>
  <LargeCardDisplay 
    v-for="largeCard in largeCardSections" 
    :key="largeCard.key"
    :cardInfo="largeCard"  
  />
  <SmallCardDisplay 
    v-for="smallCard in smallCardSections" 
    :key="smallCard.key"
    :cardInfo="smallCard"  
  />
</div>
</template>

<script>
import Introduction from '~/components/Introduction.vue'
import LargeCardDisplay from '~/components/LargeCardDisplay.vue'
import SmallCardDisplay from '~/components/SmallCardDisplay.vue'
import Navbar from '~/components/Navbar.vue'
import {largeCardSections,smallCardSections} from '~/assets/data.js'
export default {
  data(){
    return{
      largeCardSections:largeCardSections,
      smallCardSections:smallCardSections,
    }
  }
}

</script>