<template>
    <div>
        <div class="container">
        <h5>{{cardInfo.title}}</h5>
        <SmallCardImageDisplay 
            :smallCardImage="cardInfo.cards"
        />
    </div>
    </div>
</template>

<script>
    import SmallCardImageDisplay from '~/components/SmallCardImageDisplay.vue'
    export default {
        props:['cardInfo']
    }
</script>

<style scoped>

</style>