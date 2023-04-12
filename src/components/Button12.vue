<template>
    <button v-on:click="getWheel(Image)" class="btn btn-dark">
        <img v-bind:src="Image.Src">
        <p>{{ Image.Brand }}<br>{{ Image.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `Button12`,
    data() {
        return {
            Image: {
                Src: require("../assets/Rotiform-BTL.png"),
                Brand: "Rotiform",
                Name: "BTL",
            }
        }
    },
    props: {
        getWheel:Function
    }
}
</script>