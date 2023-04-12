<template>
    <button v-on:click="getWheel(Image)" class="btn btn-dark">
        <img v-bind:src="Image.Src">
        <p>{{ Image.Brand }}<br>{{ Image.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `Button7`,
    data() {
        return {
            Image: {
                Src: require("../assets/KMC-toro-forged-beadlock.png"),
                Brand: "KMC",
                Name: "Toro Forged Beadlock",
            }
        }
    },
    props: {
        getWheel:Function
    }
}
</script>