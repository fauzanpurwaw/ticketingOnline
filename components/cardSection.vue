<template>
    <div class="card">
        <div class="card-image">
            <img class="w-full max-h-96 lg:rounded-l-xl rounded" :src="image">
        </div>
        <div class="card-text">
            <p><span class="font-semibold text-xl">{{ title }} </span> {{ text }}</p>
        </div>
    </div>
</template>


<style>
.card {
    @apply lg:flex grid grid-cols-1 w-full h-full shadow-xl rounded-xl p-5 bg-white min-h-fit items-center;
}

.card-text {
    @apply flex w-full items-center text-center p-4 flex-auto lg:w-32 xl:overflow-y-hidden overflow-y-scroll; 
}

.card-image {
    @apply lg:w-64 w-full h-fit flex-auto text-center items-center;
}
</style>


<script setup>
const props = defineProps({
    title: String,
    image: String,
    text: String
})
</script>
