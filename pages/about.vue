<template>
    <div class="d-flex flex-column container-full justify-content-center align-items-center">
        
        <div class="d-flex w-100 justify-content-center">
            <div class="col-sm-7" id="retro-img-holder">
                <div id="retro-img-trail"></div>
            </div>
        </div>
        <div class="d-flex justify-content-center">
            <p class="da-fira col-sm-7 mt-3">Established in 2018, we are a company dedicated to the culture. We ensure you get your products even if they are old out in milliseconds. Whether you are an artist or a skater--Welcome!</p>
        </div>
        <div class="d-flex">
            <HomeButton/>
        </div>
    </div>
</template>

<script>
export default {
    components: {
        Return: () => import('@/components/HomeButton.vue')
    }
}
</script>

<style scoped>
.container-full {
  height: 100vh;
  width: 100vw;
}
#retro-img-holder {
    background-image: url('~@/assets/retro.webp');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    height: 400px;
}
.da-fira {
    font-family: 'Fira Code', monospace;
}
</style>