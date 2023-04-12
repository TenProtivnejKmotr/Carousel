<template>
    <button v-on:click="getWheel(Image)" class="btn btn-dark">
        <img v-bind:src="Image.Src">
        <p>{{ Image.Brand }}<br>{{ Image.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `Button3`,
    data() {
        return {
            Image: {
                Src: require("../assets/Black-rhino-arsenal-AT.png"),
                Brand: "Black Rhino",
                Name: "Arsenal AT",
            }
        }
    },
    props: {
        getWheel:Function
    }
}
</script>