<template>
    <div class="home">
        <div class="home-content">
            <h1>This is Eldoret JavaScript</h1>
            <img :src="require(`@/assets/about/${'about.jpg'}`)" alt="about">
        </div>
    </div>
</template>

<script>
export default {
    nane: "Homepage"
}
</script>

<style scoped>
    .home{
        width:100%;
        max-width: 100%;
        overflow-x: hidden;
    }
    .home img{
        width: 100%;
        z-index: 1;
    }
    .home-content h1{
        z-index: 100;
        color:#fff;
        font-family: Poppins;
        text-transform: uppercase;
        font-weight: 600;
        font-size: 4.2rem;
        position: absolute;
        top: 35%;
        left: 25%;
    }
    @media screen and (max-width: 600px) {
        .home{
            width: 100%;
            max-width: 100%;
        }
        .home-content img{
            width: 100%;
            max-width: 100%;
            height:35vh;
        }
        .home-content h1{
            display: flex;
            position: absolute;
            top: 200px;
            left: 80px;
            font-size: 2rem;
        }
    }
</style>