<template>
    <button v-for="Wheels in Image" :key="Wheels" type="button" id="Wheel" class="Wheels btn btn-light">
        <img v-bind:src="Wheels.Src">
        <p>{{ Wheels.Brand }}<br>{{ Wheels.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `WheelButton`,
    data() {
        return {
            Image: [
                {Src: require("../assets/American-Racing-Mach-Five.png"), Brand:"American Racing", Name:"Mach Five", index:1},
                {Src: require("../assets/American-racing-groove.png"), Brand:"American Racing", Name:"Groove", index:2},
                {Src: require("../assets/Black-rhino-arsenal-AT.png"), Brand:"Black Rhino", Name:"Arsenal AT", index:3},
                {Src: require("../assets/Cray-Panthera.png"), Brand:"Cray", Name:"Panthera", index:4},
                {Src: require("../assets/Fuel-Offroad-Quake.png"), Brand:"Fuel Offroad", Name:"Quake", index:5},
                {Src: require("../assets/KMC-Impact-UTV.png"), Brand:"KMC", Name:"Impact UTV", index:6},
                {Src: require("../assets/KMC-toro-forged-beadlock.png"), Brand:"KMC", Name:"Toro Forged Beadlock", index:7},
                {Src: require("../assets/KMC-Wheels-Lobo.png"), Brand:"KMC", Name:"Lobo", index:8},
                {Src: require("../assets/Motegi-Racing-S12.png"), Brand:"Motegi Racing", Name:"S12", index:9},
                {Src: require("../assets/MSA-Offroad-Wheels-Sniper.png"), Brand:"MSA Offroad Wheels", Name:"Sniper", index:10},
                {Src: require("../assets/Niche-Teramo.png"), Brand:"Niche", Name:"Teramo", index:11},
                {Src: require("../assets/Rotiform-BTL.png"), Brand:"Rotiform", Name:"BTL", index:12},
                {Src: require("../assets/XD-Specter.png"), Brand:"XD", Name:"Specter", index:13},
                {Src: require("../assets/XO-Helsinki.png"), Brand:"XO", Name:"Helsinki", index:14},
                {Src: require("../assets/Amercan-racing-Outlaw-I.png"), Brand:"American Racing", Name:"Outlaw I", index:15}
        
            ]
        }
    }
}
</script>

<style scoped>
img {
    width: 150px;
}
button {
    margin: 2px;
}
.Wheels:focus {
    background: yellow;
}
div .container {
    background: rgba(0,0,0, .25);
    width: 100%;
    height: 400px;
    border-radius: 10px;
}
</style>