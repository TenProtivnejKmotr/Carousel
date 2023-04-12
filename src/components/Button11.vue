<template>
    <button v-on:click="getWheel(Image)" class="btn btn-dark">
        <img v-bind:src="Image.Src">
        <p>{{ Image.Brand }}<br>{{ Image.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `Button11`,
    data() {
        return {
            Image: {
                Src: require("../assets/Niche-Teramo.png"),
                Brand: "Niche",
                Name: "Teramo",
            }
        }
    },
    props: {
        getWheel:Function
    }
}
</script>