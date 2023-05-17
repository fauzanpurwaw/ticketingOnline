<template>
    <div class="header">
        <div class="backdrop-blur-sm w-full h-full">
            <slot />
            <div class="header-container pt-10">
                <div class="header-content">
                    <h1 class="title">hallo, <span class="font-semibold">Selamat Datang!</span></h1>
                    <div class="search-bar">
                        <input class="search-input" type="text" placeholder="Cari Disini...">
                    </div>
                    <div class="header-list">
                        <div class="list-item">
                            <div class="p-2 rounded-full bg-slate-300 hover:bg-slate-400 mx-3">
                                <img src="/img/flight.png" alt="" class="h-10 w-10">   
                            </div>
                            <h3 class="p-1 text-slate-600 font-semibold">Title</h3>
                        </div>
                        <div class="list-item">
                            <div class="p-2 rounded-full bg-slate-300 hover:bg-slate-400 mx-3">
                                <img src="/img/flight.png" alt="" class="h-10 w-10">   
                            </div>
                            <h3 class="p-1 text-slate-600 font-semibold">Title</h3>
                        </div>
                        <div class="list-item">
                            <div class="p-2 rounded-full bg-slate-300 hover:bg-slate-400 mx-3">
                                <img src="/img/flight.png" alt="" class="h-10 w-10">   
                            </div>
                            <h3 class="p-1 text-slate-600 font-semibold">Title</h3>
                        </div>
                        <div class="list-item">
                            <div class="p-2 rounded-full bg-slate-300 hover:bg-slate-400 mx-3">
                                <img src="/img/flight.png" alt="" class="h-10 w-10">   
                            </div>
                            <h3 class="p-1 text-slate-600 font-semibold">Title</h3>
                        </div>
                        <div class="list-item">
                            <div class="p-2 rounded-full bg-slate-300 hover:bg-slate-400 mx-3">
                                <img src="/img/flight.png" alt="" class="h-10 w-10">   
                            </div>
                            <h3 class="p-1 text-slate-600 font-semibold">Title</h3>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style>
.header {
    @apply w-full bg-[url('/img/header.jpg')] bg-cover bg-center md:h-96 h-80 bg-no-repeat sticky;
}

.header-container {
    @apply flex justify-center items-center h-full w-full;
}

.header-content {
    @apply text-center w-full px-10;
}

.title {
    @apply text-3xl text-slate-600;
}

.search-bar {
    @apply p-2 rounded-3xl mt-5 w-full;
}

.search-input {
    @apply text-xl w-full rounded-xl px-3 py-2 max-w-sm;
}

.header-list {
    @apply  flex justify-center text-center w-full px-10 my-5;   
}

.list-item {
    @apply list-none text-center mt-2 min-w-fit hidden md:block;
}
</style>

<script>

</script>