<template>
    <div class="container">
        <h5 class="mt-5">{{smallCardData.title}}</h5>
        <div class="row">
            <div class="col-md-4" v-for="card in smallCardData.cards" :key="card.id">
            <NuxtLink :to="`/products/${card.id}`">
                <div class="card" style="width: 18rem;">
                    <img :src="require(`~/assets/images/${card.image}`)" class="card-img-top" alt="...">
                </div>
            </NuxtLink>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        props:['smallCardData']
    }
</script>

<style scoped>
    img{
        height: 150px;
    }
</style>