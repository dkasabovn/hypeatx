<template>
  <div class="d-flex container-fluid justify-content-center align-items-center container-full" >
    <div class="d-flex flex-column">
      <div class="big d-flex" id="one">
        <h1>HYPE</h1>
      </div>
      <div class="d-flex flex-row atx-container justify-content-between" id="animation-target">
        <div class="d-flex flex-column justify-content-around">
          <div class="d-flex flex-row" id="one-cont">
            <router-link id="one-one" class="mb-0" tag="p" to="/about">ABOUT</router-link>
            <router-link class="mb-0" tag="p" to="/contact">CONTACT US</router-link>
          </div>
          <div class="d-flex flex-row">
            <p class="mb-0" id="one-two">COMING BACK</p>
            <p class="mb-0">MAR 2021</p>
          </div>
        </div>
        <div class="mid">
          <h1>ATX</h1>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.big h1 {
  font-family: 'Work Sans', sans-serif;
  font-weight: 800;
  font-size: 320px;
  line-height: .7em;
}
/* .big h1::before {
  position: absolute;
  content: '';
  right: .91em;
  top: 22%;
  display: inline-block;
  background-color: #212529;
  width: 63px;
  height: 60px;
} */
.atx-container {
  padding-left: 20px;
}
.mid h1 {
  font-family: 'Work Sans', sans-serif;
  font-size: 170px;
  line-height: .7em;
}
.container-full {
  height: 100vh;
  width: 100vw;
}
p {
  font-family: 'Work Sans';
  text-decoration: underline;
  font-size: 30px;
}
#one-one::after {
  content: '';
  display: inline-block;
  width: 180px;
  bottom: 5%;
  margin: 0 10px;
  height: 5px;
  position: relative;
  background: rgb(131,58,180);
  background: linear-gradient(67deg, rgba(131,58,180,1) 0%, rgba(253,29,29,1) 50%, rgba(252,176,69,1) 100%);
}
#one-two::after {
  content: '';
  display: inline-block;
  width: 120px;
  bottom: 5%;
  margin: 0 10px;
  height: 5px;
  position: relative;
  background: rgb(131,58,180);
  background: linear-gradient(67deg, rgba(131,58,180,1) 0%, rgba(253,29,29,1) 50%, rgba(252,176,69,1) 100%);
}
#one-cont p:hover {
  cursor: pointer;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  50% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
#animation-target {
  animation: 4s ease-out 0s 1 fadeIn;
}
#one {
  animation: 2s ease-out 0s 1 fadeIn;
}
</style>
