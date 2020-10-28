<template>
    <div class="container-full d-flex flex-column justify-content-center align-items-center">
        <form action="https://formspree.io/f/xaylovyb" method="POST" class="d-flex flex-column mb-5" v-if="!submitted" target="_blank">
            <input type="text" name="name" placeholder="You">
            <input type="email" name="_replyto" placeholder="your@email">
            <input type="submit" @click="submitted=true" value="SEND">
        </form>
        <h1 v-if="submitted">Thank you!</h1>
        <Home/>
    </div>
</template>

<script>
export default {
    data() {
        return {
            submitted: false
        }
    },
    components: {
        Home: () => import('@/components/HomeButton.vue')
    }
}
</script>

<style scoped>
.container-full {
  height: 100vh;
  width: 100vw;
}
h1 {
    font-family: 'Work Sans', sans-serif;
    font-size: 100px;
}
input[type="text"], input[type="email"] {
    margin-bottom: 5vh;
    font-family: 'Work Sans', sans-serif;
    border: none;
    border-bottom: 2px solid black;
    font-size: 100px;
}
input[type="submit"] {
    margin: 0;
    font-family: 'Fira Code', monospace!important;
    border: none;
    background-color: orangered;
    color: white;
    width: 30%;
}
</style>