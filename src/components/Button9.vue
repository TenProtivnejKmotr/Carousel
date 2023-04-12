<template>
    <button v-on:click="getWheel(Image)" class="btn btn-dark">
        <img v-bind:src="Image.Src">
        <p>{{ Image.Brand }}<br>{{ Image.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `Button9`,
    data() {
        return {
            Image: {
                Src: require("../assets/Motegi-Racing-S12.png"),
                Brand: "Motegi Racing",
                Name: "S12",
            }
        }
    },
    props: {
        getWheel:Function
    }
}
</script>