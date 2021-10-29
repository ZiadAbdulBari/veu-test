<template>
    <div>
        <Navbar/>
        <div class="container">
            <div class="row mt-3" v-if="product">
                <div class="col-md-6">
                    <img class="img-fluid" :src="require(`~/assets/images/${product.image}`)" alt="">
                </div>
                <div class="col-md-6">
                    <h3>{{product.title}}</h3>
                    <p>{{product.snippet}}</p>
                </div>
                <p class="mt-5 mb-5">{{product.description}}</p>

                <h4 class="mb-5">Customer review</h4>
                <Review/>
            </div>
            <div v-else >
                <h2>404!Page Not Found</h2>
            </div>
        </div>
    </div>
</template>

<script>
    
    import Review from "~/components/Review.vue"
    export default {
        computed:{
            product(){
                return this.$store.getters.getProductById(this.$route.params.id)
            }
        }
    }
</script>

<style scoped>
    .row{
        align-items: center;
    }
   
    img{
        border-radius: 5px;
    }
</style>