<template>
    <div class="container">
        <div class="row" v-for="commant in commants" :key="commant.id">
            <div class="col-md-1">
                <img :src="commant.picture.thumbnail" alt="">
            </div>
            <div class="col-md-11">
                <h5>{{commant.name.first}} {{commant.name.last}}</h5>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto harum beatae animi, maiores fuga blanditiis dolores voluptatum quidem.</p>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data(){
            return{
                commants:[]
            }
        },
        created(){
            this.getComments()
        },
        methods:{
            getComments(){
               let url="?results=5"
                this.$axios.get(url)
                    .then(res=>{
                        this.commants=res.data.results
                        console.log(res.data.results)
                    })
            }
        }
    }
</script>

<style scoped>
    img{
        border-radius: 50px;
    }
</style>