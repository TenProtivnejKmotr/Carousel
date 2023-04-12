<template>
    <button v-on:click="getWheel(Image)" class="btn btn-dark">
        <img v-bind:src="Image.Src">
        <p>{{ Image.Brand }}<br>{{ Image.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `Button13`,
    data() {
        return {
            Image: {
                Src: require("../assets/XD-Specter.png"),
                Brand: "XD",
                Name: "Specter",
            }
        }
    },
    props: {
        getWheel:Function
    }
}
</script>