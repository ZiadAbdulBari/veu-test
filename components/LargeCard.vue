<template>
    <div class="largeCard container">
        <h4>{{largeCardData.title}}</h4>
        <div class="row">
            <div class="col-md-4" v-for="card in largeCardData.cards" :key="card.id">
                <div class="card" style="width: 18rem;">
                    <img :src="require(`~/assets/images/${card.image}`)" class="card-img-top" alt="...">
                    <div class="card-body">
                        <h5 class="card-title">{{card.title}}</h5>
                        <p class="card-text">{{card.snippet}}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        props:['largeCardData']
    }
    
</script>

<style scoped>
    .largeCard{
        margin-top: 100px;
    }
    img{
        height: 200px;
    }
</style>