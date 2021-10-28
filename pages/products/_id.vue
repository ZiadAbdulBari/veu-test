<template>
    <div class="container">
        <!-- <img :src="require(`~/assets/images/${slugData.image}`)" alt=""> -->
    </div>
</template>

<script>
    import {smallCardSections} from '~/assets/data.js'
    export default {
        data(){
            return{
                slugData:[],
                smallCardData:smallCardSections[0],
            }
        },
        // created() {
        //     this.showSlugData()
        // },
        // methods:{
        //     showSlugData(){
        //         this.slugData = this.smallCardData.cards.find(img=>img.id==this.$route.params.id)
        //         console.log(this.slugData)
        //     }
        // }
    }
</script>

<style scoped>
    img{
        width: 400px;
        height: auto;
    }
</style>