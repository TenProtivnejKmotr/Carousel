<template>
  <div>
    <h1>CAR CONFIGURATION</h1>
      <div class="card text-white bg-dark">
        <div v-if="ShowData">
            <p class="textBox">{{ WheelActive.Brand }}<br>{{ WheelActive.Name }}</p>
          <img class="w-100" v-bind:src="WheelActive.Src">
        </div>
      </div>
    <div id="carouselExampleControls" class="carousel slide" data-ride="carousel"  data-interval="0">
      <div class="carousel-inner">
        <div class="carousel-item active">
          <Button1 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button1>
          <Button2 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button2>
          <Button3 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button3>
          <Button4 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button4>
          <Button5 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button5>
        </div>
        <div class="carousel-item">
          <Button6 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button6>
          <Button7 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button7>
          <Button8 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button8>
          <Button9 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button9>
          <Button10 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button10>
        </div>
        <div class="carousel-item">
          <Button11 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button11>
          <Button12 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button12>
          <Button13 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button13>
          <Button14 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button14>
          <Button15 class="bttns" v-on:focusin="ShowData = !ShowData" v-on:focusout="ShowData = !ShowData" :getWheel="getWheelActive"></Button15>
        </div>
      </div>
      <button class="carousel-control-prev" href="#carouselExampleControls" data-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
      </button>
      <button class="carousel-control-next" href="#carouselExampleControls" data-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
      </button>
    </div>
  </div>
</template>

<script>
import Button1 from './components/Button1.vue'
import Button2 from './components/Button2.vue'
import Button3 from './components/Button3.vue'
import Button4 from './components/Button4.vue'
import Button5 from './components/Button5.vue'
import Button6 from './components/Button6.vue'
import Button7 from './components/Button7.vue'
import Button8 from './components/Button8.vue'
import Button9 from './components/Button9.vue'
import Button10 from './components/Button10.vue'
import Button11 from './components/Button11.vue'
import Button12 from './components/Button12.vue'
import Button13 from './components/Button13.vue'
import Button14 from './components/Button14.vue'
import Button15 from './components/Button15.vue'

export default {
  name: 'App',
  components: {
    Button1,
    Button2,
    Button3,
    Button4,
    Button5,
    Button6,
    Button7,
    Button8,
    Button9,
    Button10,
    Button11,
    Button12,
    Button13,
    Button14,
    Button15,
  },
    methods: {
      getWheelActive(Wheels){
      this.WheelActive=Wheels
    }
  },
  data() {
    return {
      WheelActive: '',
      ShowData: false
    }
  }
}

</script>

<style>
h1 {
  margin-top: 5%;
  margin-left: 5%;
  text-align: left;
  color: #FFF;
}
img {
  width: 200px;
}
div {
  height: 100%;
}
div .bttns {
  margin: 0 2px;
  height: 300px;
  background-image: linear-gradient(rgb(119, 119, 119), rgb(26, 26, 26));
  font-size: x-large;
}
.bttns:focus {
  background-image: linear-gradient(rgb(238, 143, 0), rgb(119, 67, 0));
}
.bg-dark {
  height: 300px;
}
.carousel {
  margin-top: 50px;
}
.carousel-item {
  text-align: center;
  background: rgba(0, 0, 0, 0.8);
}
div .card {
  width: 300px;
  height: 450px;
  border-radius: 2px;
  text-align: center;
  margin-left: 5%;
  background-image: linear-gradient(rgb(119, 119, 119), rgb(26, 26, 26));
}
.carousel-control-prev, .carousel-control-next  {
  background: none;
  border: none;
}
.carousel-control-prev-icon, .carousel-control-next-icon {
  height: 50px;
  width: 50px;
}
body {
  background: url("../src/assets/cargarage.png");
  background-repeat: no-repeat;
  background-size: 110%;
  font-family: 'Teko', sans-serif;
  }
.textBox {
  background-color: rgba(0,0,0,.25);
  height: 70px;
  font-size: x-large;
}
ul.checkmark li {
  font-size: 16px;
  list-style-type: none;
  margin-bottom: 1em;
  padding: 0.25em 0 0 2.5em;
  position: relative;
  left: 80%;
  top: 10px;
}
ul.checkmark li:before {
  content: " ";
  display: block;
  border: solid 0.8em #60c90b;
  height: 0;
  width: 0;
  position: absolute;
  left: 0.5em;
  top: 40%; 
  margin-top: -0.5em;
}
ul.checkmark li:after {
  content: " ";
  display: block;
  width: 0.3em;
  height: 0.6em;
  border: solid white;
  border-width: 0 0.2em 0.2em 0;
  position: absolute;
  left: 1em;
  top: 40%;
  margin-top: -0.2em;
  -webkit-transform: rotate(45deg);
  -moz-transform: rotate(45deg);
  -o-transform: rotate(45deg);
  transform: rotate(45deg);
}
</style>
