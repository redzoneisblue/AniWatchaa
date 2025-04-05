<script setup>
import {ref} from 'vue'

const video = ref('tv/94605/2/1')
const embedUrl = `https://vidlink.pro/${video.value}?primaryColor=ff0000&secondaryColor=a2a2a2&iconColor=eefdec&icons=default&player=default&title=true&poster=true&autoplay=false&nextbutton=false`
console.log(video.value)

</script>

<template>

    <iframe :src="embedUrl" frameborder="0"></iframe>

</template> 

<style lang="scss" scoped>
iframe {
    scale: 2;
}
</style>