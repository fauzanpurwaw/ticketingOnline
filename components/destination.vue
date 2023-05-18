<template>
    <div class="destination flex w-full">
        <div class="destination-content w-full">
            <div class="judul">
                <h1 class="text-2xl font-semibold text-left">Nginep asyik di destinasi favorit.</h1>
                <p class="text-left">Saatnya kasih reward ke diri sendiri dengan rileks di hotel di berbagai destinasi
                    domestik menarik.</p>
            </div>
            <div class="flex mt-10 gap-3 lg:overflow-hidden overflow-x-auto">
                <div class="destination-item text-left">
                    <NuxtLink to="destinasi/bali">
                        <img class="w-full rounded-xl" src="/img/bali.webp" alt="">
                        <h2 class="font-semibold text-lg sm:text-left text-center">Bali</h2>
                        <div class="flex w-full">
                            <p>Ekonomi</p>
                            <h3 class="float-right w-full text-right">Rp.100.000,-</h3>
                        </div>
                    </NuxtLink>
                </div>
                <div class="destination-item text-left">
                    <NuxtLink to="destinasi/bandung">
                        <img class="w-full rounded-xl" src="/img/bandung.webp" alt="">
                        <h2 class="font-semibold text-lg sm:text-left text-center">Bandung</h2>
                        <div class="flex w-full">
                            <p>Ekonomi</p>
                            <h3 class="float-right w-full text-right">Rp.100.000,-</h3>
                        </div>
                    </NuxtLink>
                </div>
                <div class="destination-item text-left">
                    <NuxtLink to="destinasi/jakarta">
                        <img class="w-full rounded-xl" src="/img/jakarta.webp" alt="">
                        <h2 class="font-semibold text-lg sm:text-left text-center">Jakarta</h2>
                        <div class="flex w-full">
                            <p>Ekonomi</p>
                            <h3 class="float-right w-full text-right">Rp.100.000,-</h3>
                        </div>
                    </NuxtLink>
                </div>
                <div class="destination-item text-left">
                    <NuxtLink to="destinasi/surabaya">
                        <img class="w-full rounded-xl" src="/img/surabaya.webp" alt="">
                        <h2 class="font-semibold text-lg sm:text-left text-center">Surabaya</h2>
                        <div class="flex w-full">
                            <p>Ekonomi</p>
                            <h3 class="float-right w-full text-right">Rp.100.000,-</h3>
                        </div>
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
    @apply p-10 ;
}

.judul {
    @apply w-full;
}

</style>

<script>
</script>