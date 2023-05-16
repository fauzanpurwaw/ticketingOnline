<template>
    <div class="card">
        <div class="card-image">
            <img class="w-full h-full" :src="image">
        </div>
        <div class="card-text">
            <p><span>Text</span> {{ text }}</p>
        </div>
    </div>
</template>


<style>
.card {
    @apply md:flex grid grid-cols-1 w-full h-full shadow-xl rounded-xl p-5 bg-white max-h-fit ;
}

.card-text {
    @apply flex w-full items-center text-center p-4 flex-auto md:w-32 text-center; 
}

.card-image {
    @apply rounded-l-xl md:w-64 w-full h-full flex-auto text-center;
}
</style>


<script setup>
const props = defineProps({
    image: String,
    text: String
})
</script>
