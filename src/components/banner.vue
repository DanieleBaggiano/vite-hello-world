<script>
import { ref } from 'vue'

export default {
    data() {
        return {
            imageName: "Moscardini-alla-Luciana.avif"
        };
    },
    methods: {
        getImagePath(img) {
            return new URL(`../assets/${img}`, import.meta.url).href;
        }
    },
};
</script>

<template>
  <div>
    <img :src="getImagePath(imageName)">
  </div>
</template>

<style scoped>

</style>