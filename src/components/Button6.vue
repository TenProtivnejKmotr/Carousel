<template>
    <button v-on:click="getWheel(Image)" class="btn btn-dark">
        <img v-bind:src="Image.Src">
        <p>{{ Image.Brand }}<br>{{ Image.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `Button6`,
    data() {
        return {
            Image: {
                Src: require("../assets/KMC-Impact-UTV.png"),
                Brand: "KMC",
                Name: "Impact UTV",
            }
        }
    },
    props: {
        getWheel:Function
    }
}
</script>