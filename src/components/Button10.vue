<template>
    <button v-on:click="getWheel(Image)" class="btn btn-dark">
        <img v-bind:src="Image.Src">
        <p>{{ Image.Brand }}<br>{{ Image.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `Button10`,
    data() {
        return {
            Image: {
                Src: require("../assets/MSA-Offroad-Wheels-Sniper.png"),
                Brand: "MSA Offroad Wheels",
                Name: "Sniper",
            }
        }
    },
    props: {
        getWheel:Function
    }
}
</script>