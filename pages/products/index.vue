<template>
    <div>
        <LargeCard
            v-for="largeCard in largeCardData" 
            :key="largeCard.id" 
            :largeCardData="largeCard"
        />
    </div>
</template>

<script>
    import LargeCard from '~/components/LargeCard.vue'
    import {largeCardSections} from '~/assets/data.js'
    export default {
        data(){
            return{
                largeCardData:largeCardSections
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>