<template>
    <button v-on:click="getWheel(Image)" class="btn btn-dark">
        <img v-bind:src="Image.Src">
        <p>{{ Image.Brand }}<br>{{ Image.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `Button8`,
    data() {
        return {
            Image: {
                Src: require("../assets/KMC-Wheels-Lobo.png"),
                Brand: "KMC",
                Name: "Lobo",
            }
        }
    },
    props: {
        getWheel:Function
    }
}
</script>