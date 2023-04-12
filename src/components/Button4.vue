<template>
    <button v-on:click="getWheel(Image)" class="btn btn-dark">
        <img v-bind:src="Image.Src">
        <p>{{ Image.Brand }}<br>{{ Image.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `Button4`,
    data() {
        return {
            Image: {
                Src: require("../assets/Cray-Panthera.png"),
                Brand: "Cray",
                Name: "Panthera",
            }
        }
    },
    props: {
        getWheel:Function
    }
}
</script>