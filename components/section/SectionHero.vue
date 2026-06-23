<template>
    <div class="flex w-full justify-center">
        <div class="md:h-[85vh] h-[26vh] bg-red-500 md:w-[1366px] w-full">
            <img src="/hero1.webp" class="w-full h-full object-fit">
        </div>
    </div>
</template>
<script setup>
const props = defineProps({
    src: String,
})
</script>
