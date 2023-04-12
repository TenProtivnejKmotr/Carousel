<template>
    <button v-on:click="getWheel(Image)" class="btn btn-dark">
        <img v-bind:src="Image.Src">
        <p>{{ Image.Brand }}<br>{{ Image.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `Button5`,
    data() {
        return {
            Image: {
                Src: require("../assets/Fuel-Offroad-Quake.png"),
                Brand: "Fuel Offroad",
                Name: "Quake",
            }
        }
    },
    props: {
        getWheel:Function
    }
}
</script>