<template>
    <button v-on:click="getWheel(Image)" class="btn btn-dark">
        <img v-bind:src="Image.Src">
        <p>{{ Image.Brand }}<br>{{ Image.Name }}</p>
    </button>
</template>

<script>
export default{
    name: `Button14`,
    data() {
        return {
            Image: {
                Src: require("../assets/XO-Helsinki.png"),
                Brand: "XO",
                Name: "Helsinki",
            }
        }
    },
    props: {
        getWheel:Function
    }
}
</script>