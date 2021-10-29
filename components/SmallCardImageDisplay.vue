<template>
    <div>
        <div class="container">
        <div class="row">
            <div class="col-md-2" v-for="cardImage in smallCardImage" :key="cardImage.id">
                <NuxtLink :to="`/product/${cardImage.id}`">
                    <div class="card" style="width: 10rem">
                        <img :src="require(`~/assets/images/${cardImage.image}`)" alt="">
                    </div>
                </NuxtLink>
            </div>
        </div>
    </div>
    </div>
</template>

<script>
    export default {
        props:['smallCardImage']
    }
</script>

<style scoped>
    img{
        height: 120px;
    }
</style>