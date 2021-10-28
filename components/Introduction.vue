<template>
    <div>
        <div class="container">
            <div class="row mt-3">
                <div class="col-md-8">
                    <h1>Find your Fire Extinguisher</h1>
                    <p class="snippet">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Iste iusto illum quidem asperiores, cum nisi aperiam eius ipsa sapiente odit!</p>
                    <button class="button btn">Start Looking</button>
                </div>
                <div class="col-md-4">
                    <img class="image" src="~assets/svg/fire-extinguisher.svg" alt="fire extinguisher">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .row{
        align-items: center;
    }
    .text-container {
        width: 50%;
        margin-top: 4rem;
    }
    
    .snippet {
        color: grey;
        font-size: 1.25rem;
    }
    .image {
        width: 300px;
        height: auto;
        /* margin-top: 2rem; */
    }
    
    .button {
        padding: 1rem 4rem;
        border-radius: 100rem;
        background-color: rgb(231, 81, 43);
        color: white;
        width: 20rem;
        font-weight: 700;
        transition: 0.5s;
    }
    .button:hover {
        width: 21.5rem;
    }
    @media (max-width: 500px) {
        .Hero {
            height: 40vh;
        }
    }
</style>