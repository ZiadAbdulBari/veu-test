<template>
    <div class="container">
        <h5>{{cardInfo.title}}</h5>
        <LargeCardImageDisplay 
            :largeCardImage="cardInfo.cards"
        />
    </div>
</template>

<script>
    import LargeCardImageDisplay from '~/components/LargeCardImageDisplay.vue'
    export default {
        props:['cardInfo']
    }
</script>

<style scoped>

</style>