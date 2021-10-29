<template>
    <div>
        <nav class="navbar navbar-expand-lg navbar-light bg-dark">
            <div class="container-fluid">
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                        <li class="nav-item">
                            <nuxtLink class="nav-link active" aria-current="page" to="/">Home</nuxtLink>
                        </li>
                        <li class="nav-item">
                            <nuxtLink class="nav-link active" aria-current="page" to="/product">Product</nuxtLink>
                        </li>
                        <li class="nav-item">
                            <nuxtLink class="nav-link active" aria-current="page" to="/myitem">My item</nuxtLink>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>

</style>