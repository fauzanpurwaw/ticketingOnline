<template>
    <div class="container mx-auto">
        <div class="content px-9">
            <div class="header mt-16">
                <h1 class="md:text-3xl mx-8 text-center text-2xl">Hello!, Here I'll Show You How To Make an Omelette
                </h1>
            </div>
            <div class="section w-full mt-16 ">
                <div class="md:flex grid grid-cols-1">
                    <div class="flex-auto md:w-64 w-98 m-9">
                        <img class="w-full h-full rounded-xl"
                            src="https://img.freepik.com/free-photo/tasty-omelette-tomato-slices-white-plate_114579-73850.jpg?w=826&t=st=1683692086~exp=1683692686~hmac=d77dc7bdcf9c03fe1877648fa7847114fae9d176f15c830fdec0cdcd8a7e4fe2"
                            alt="">
                    </div>
                    <div class="flex flex-auto md:w-32 w-98 text-justify items-center px-9">
                        <p>
                            <span class="text-xl font-semibold">Omelette</span> is a dish made from beaten eggs, fried
                            with butter or oil in a frying pan
                            (without stirring as in scrambled egg).
                        </p>
                    </div>
                </div>
            </div>
            <div class="section w-full mt-16">
                <div class="md:flex grid grid-cols-1">
                    <div class="md:flex-auto md:w-64 w-98 m-9">
                        <h2 class="text-xl font-semibold text-center underline hover:text-lg">Ingredients</h2>
                        <div class="grid grid-cols-2 gap-1 text-center mt-9 h-full">
                            <div class="col flex items-center justify-center border p-3 border-black rounded">
                                Eggs
                            </div>
                            <div class="col flex items-center justify-center border p-3 border-black rounded">
                                2
                            </div>
                            <div class="col flex items-center justify-center border p-3 border-black rounded">
                                Salt
                            </div>
                            <div class="col flex items-center justify-center border p-3 border-black rounded">
                                2 tsb (30ml)
                            </div>
                            <div class="col flex items-center justify-center border p-3 border-black rounded">
                                Pepper
                            </div>
                            <div class="col flex items-center justify-center border p-3 border-black rounded">
                                Just A Pinch
                            </div>
                            <div class="col flex items-center justify-center border p-3 border-black rounded">
                                Filling Ingredients
                            </div>
                            <div class="col flex items-center justify-center border p-3 border-black rounded">
                                Just Fill With All u Want
                            </div>
                        </div>
                    </div>
                    <div class="md:flex-auto md:w-64 w-98 m-9 md:mt-0 mt-16">
                        <h2 class="text-xl font-semibold text-center underline hover:text-lg">Instruction</h2>
                        <div class="card border border-black rounded text-center mt-9 min-h-fit h-full">
                            <div class="instruction px-6">
                                <h3 class="text-sm py-5">Step 1</h3>
                                <p class="text-center mb-3">
                                    Whisk eggs, water, salt and pepper.
                                </p>
                            </div>
                            <div class="instruction px-6">
                                <h3 class="text-sm py-5">Step 2</h3>
                                <p class="text-center mb-3">
                                    Spray 8-inch (20 cm) non-stick skillet with cooking spray. Heat over medium heat.
                                    Pour in egg mixture. As eggs set around edge of skillet, with spatula, gently push
                                    cooked portions toward centre of skillet. Tilt and rotate skillet to allow uncooked
                                    egg to flow into empty spaces.
                                </p>
                            </div>
                            <div class="instruction px-6">
                                <h3 class="text-sm py-5">Step 3</h3>
                                <p class="text-center mb-3">
                                    When eggs are almost set on surface but still look moist, cover half of omelette
                                    with filling. Slip spatula under unfilled side; fold over onto filled half.
                                </p>
                            </div>
                            <div class="instruction px-6">
                                <h3 class="text-sm py-5">Step 4</h3>
                                <p class="text-center mb-3">
                                    Cook for a minute, then slide omelette onto plate.
                                </p>
                            </div>
                        </div>
                        <!-- <div class="grid grid-cols-2 gap-2">
                            <button class="w3-button w3-black w3-display-left" onclick="ganti(-1)">&#10094;</button>
                            <button class="w3-button w3-black w3-display-right" onclick="ganti(1)">&#10095;</button>
                        </div> -->
                    </div>
                </div>
            </div>
            <div class="section video mt-16 mx-auto">
                <h2 class="text-xl font-semibold text-center underline hover:text-lg">Video</h2>
                <iframe class="mt-5 rounded-xl" width="100%" height="315px" src="https://www.youtube.com/embed/y-Wr401Bio4"
                    title="YouTube video player" frameborder="0"
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                    allowfullscreen></iframe>
            </div>
        </div>
        <a href="#">
            <div class="footer border border-black rounded-xl p-3 mt-10 mb-5 text-center hover:font-semibold">
                Create by Fauzan &copy;copyright
            </div>
        </a>
    </div>
</template>

<style>
body {
    @apply font-mono bg-yellow-500;
}

.instruction {
    display: block;
}

.card {
    position: relative;
    display: block;
}

.video {
    max-width: 680px;
}
</style>



