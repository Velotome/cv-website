<script setup>  
    const props = defineProps({
        img_name: {
            type: String,
            default: "placeholder"
        }
    })
    const imageUrl = new URL(`/src/assets/${props.img_name}.png`, import.meta.url).href
    console.log(imageUrl)
</script>

<template>
    <div 
    class="flex flex-row gap-10 md:mx-10 columns-2 bg-green-800 bg-opacity-80 rounded md:px-4 md:py-4">
        <img :src="imageUrl" alt="nyaaa" class="rounded basis-1/3">
        
        <div class="text-white basis-2/3">
            Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
        </div>
    </div>
</template>
