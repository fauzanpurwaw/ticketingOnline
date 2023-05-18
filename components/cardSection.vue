<template>
    <div class="card w-full h-full flex justify-center items-center">
        <div class="card-content flex lg:flex-nowrap flex-wrap justify-center items-center w-full h-full">
            <div class="card-img h-full w-full lg:mr-10 sm:px-0 px-10 flex justify-center">
                <img :src="image" alt="" class="">
            </div>
            <div class="card-text w-full h-full text-left">
                <h1 class="text-2xl font-semibold py-10">{{ title }}</h1>
                <p><span class="font-bold">Lorem ipsum dolor sit amet.</span>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat nam, quidem illum veritatis vero maxime
                    cumque qui corporis? Provident itaque consectetur aliquid. Incidunt eos consequuntur quos quibusdam amet
                    assumenda itaque, et obcaecati velit suscipit sunt facere inventore culpa voluptate ab?</p>
                <br>
                <p>
                    <span class="font-bold">Lorem ipsum dolor sit amet consectetur.</span>
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ad exercitationem delectus adipisci rem quia
                    ab sapiente aut inventore! Alias placeat aliquam repellat, nulla illum reprehenderit.
                </p>
            </div>
        </div>
    </div>
</template>


<style>
.card-content {
    @apply p-10;
}
</style>


<script setup>
const props = defineProps({
    title: String,
    image: String,
})
</script>
