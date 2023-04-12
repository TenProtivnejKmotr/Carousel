<template>
    <button v-on:click="getWheel(Image)" class="btn btn-dark">
        <img v-bind:src="Image.Src">
        <p>{{ Image.Brand }}<br>{{ Image.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `Button1`,
    data() {
        return {
            Image: {
                Src: require("../assets/American-Racing-Mach-Five.png"),
                Brand: "American Racing",
                Name: "Mach Five",
            }
        }
    },
    props: {
        getWheel:Function
    }
}
</script>