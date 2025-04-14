<script setup>
import {ref} from 'vue'

const video = ref({
    title: "yao-shen-ji-8th-season-2024",
    epNo: "23"
})
// const embedUrl = `https://anime.autoembed.cc/embed/${video.title}-episode-${video.number}`
// console.log(video.value)
const embedUrl = `https://anime.autoembed.cc/embed/yao-shen-ji-8th-season-2024-episode-23`
console.log(video.value)

</script>

<template>

    <iframe :src="embedUrl" frameborder="0"></iframe>

</template> 

<style lang="scss" scoped>
iframe {
    position: relative;
    top: 15rem;
    scale: 2;
    align-self: center;
}
</style>