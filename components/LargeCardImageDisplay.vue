<template>
    <div class="container">
        <div class="row">
            <div class="col-md-4" v-for="cardImage in largeCardImage" :key="cardImage.id">
                <NuxtLink :to="`/product/${cardImage.id}`">
                    <div class="card" style="width: 18rem;">
                        <img :src="require(`~/assets/images/${cardImage.image}`)" alt="">
                        <div class="card-body">
                            <h5 class="card-title">{{cardImage.title}}</h5>
                            <p class="card-text">{{cardImage.snippet}}</p>
                        </div>
                    </div>
                </NuxtLink>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        props:['largeCardImage']
    }
</script>

<style scoped>
    img{
        height: 250px;
    }
</style>