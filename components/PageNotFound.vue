<template>
    <div>
        <h1>
            Page Not Found <br>
            <Nuxt-Link to="/">Go to home page</Nuxt-Link>
        </h1>
        
        <img :src="require('@/assets/images/fe25.jpg')" alt="">
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    div {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 50rem;
        margin: 0 auto;
    }
    h1 {
        font-size: 5.5rem;
    }
    img {
        width: 15rem;
        margin: 0 auto
    }
    a {
        font-size: 3.5rem
    }
</style>