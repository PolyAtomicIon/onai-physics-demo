<script setup lang="ts">
import { ref } from 'vue'

const props = defineProps({
    src: {
        default: '',
    },
    applyStyle: {
        default: true
    },
    height: {
        default: '370px'
    },
    width: {
        default: '100%'
    },
})

</script>

<template>
    <div class="iframe-container" :style="`height: ${props.height}; width: ${props.width}`">
        <iframe 
            :src="props.src" 
            frameborder="0"
            :class="props.applyStyle ? 'iframe--specific-part' : 'iframe--full'"
        ></iframe>
    </div>
</template>


<style scoped>
.iframe-container {
    /* background-color: aqua; */
    overflow: hidden;
    position: relative;
}

.iframe--full {
    width: 100%;
    height: 100%;
}

.iframe--specific-part {
    /* position: absolute;
    top: 0;
    left: 0; */
    border: 0px none; 
    margin-left: 0px; 
    margin-top: -125px; 
    height: 525px; 
    width: 900px;
}
</style>