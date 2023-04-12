<template>
    <button v-on:click="getWheel(Image)" class="btn btn-dark">
        <img v-bind:src="Image.Src">
        <p>{{ Image.Brand }}<br>{{ Image.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `Button15`,
    data() {
        return {
            Image: {
                Src: require("../assets/Amercan-racing-Outlaw-I.png"),
                Brand: "American Racing",
                Name: "Outlaw I",
            }
        }
    },
    props: {
        getWheel:Function
    }
}
</script>