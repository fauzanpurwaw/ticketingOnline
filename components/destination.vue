<template>
    <div class="destination">
        <div class="destination-content">
            <div class="judul">
                <h1 class="text-2xl font-semibold text-left">Nginep asyik di destinasi favorit.</h1>
                <p class="text-left">Saatnya kasih reward ke diri sendiri dengan rileks di hotel di berbagai destinasi
                    domestik menarik.</p>
            </div>
            <div class="grid grid-cols-4 gap-2 mt-10">
                <div class="destination-item text-left">
                    <NuxtLink to="destinasi/bali">
                        <img class="w-full h-64 rounded-xl" src="/img/bali.webp" alt="">
                        <h2 class="font-semibold text-lg">Bali</h2>
                    </NuxtLink>
                </div>
                <div class="destination-item text-left">
                    <NuxtLink to="destinasi/bandung">
                        <img class="w-full h-64 rounded-xl" src="/img/bandung.webp" alt="">
                        <h2 class="font-semibold text-lg">Bandung</h2>
                    </NuxtLink>
                </div>
                <div class="destination-item text-left">
                    <NuxtLink to="destinasi/jakarta">
                        <img class="w-full h-64 rounded-xl" src="/img/jakarta.webp" alt="">
                        <h2 class="font-semibold text-lg">Jakarta</h2>
                    </NuxtLink>
                </div>
                <div class="destination-item text-left">
                    <NuxtLink to="destinasi/surabaya">
                        <img class="w-full h-64 rounded-xl" src="/img/surabaya.webp" alt="">
                        <h2 class="font-semibold text-lg">Surabaya</h2>
                    </NuxtLink>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
.destination {
    @apply w-full;
}

.destination-content {
    @apply p-10;
}

.judul {
    @apply w-full;
}
</style>

<script>
</script>