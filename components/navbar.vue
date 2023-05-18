<template>
    <nav class="bg-transparen w-full">
        <div class="mx-auto max-w-7xl sm:px-6 lg:px-8 w-full">
            <div class="relative flex h-16 items-center justify-between">
                <div class="flex flex-1 items-center w-full justify-center md:justify-start">
                    <div class="items-center hidden sm:block">
                        <div class="flex w-full h-8 sm:ml-0 ml-3">
                            <p class="inline lg:text-xl tedt-sm text-slate-200">
                                tiket
                                <span>
                                    <div class="mt-1 inline-block w-5 h-5 rounded-full bg-yellow-400"></div>
                                 </span>
                                com
                            </p>
                        </div>
                    </div>
                    <div class="sm:ml-12 ml-0">
                        <div class="flex space-x-4 w-full">
                            <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
                            <NuxtLink to="/"
                             class="text-slate-200 hover:underline rounded-md px-3 py-2 text-sm font-medium">
                                Dashboard
                            </NuxtLink>
                            <NuxtLink to="/destinasi"
                             class="text-slate-200 hover:underline rounded-md px-3 py-2 text-sm font-medium">
                                Destinasi
                            </NuxtLink>
                            <NuxtLink 
                             class="text-slate-200 hover:underline rounded-md px-3 py-2 text-sm font-medium">
                                ASAP
                            </NuxtLink>
                            <NuxtLink
                             class="text-slate-200 hover:underline rounded-md px-3 py-2 text-sm font-medium">
                                ASAP
                            </NuxtLink>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </nav>
</template>
