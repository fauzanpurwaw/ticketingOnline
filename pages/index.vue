<template>
    <div class="container mx-auto">
        <div class="content mx-auto w-fit px-9">
            <NuxtLayout :name="layouts.header">
                Hello, here I'll Show You How To Make an Omelette
            </NuxtLayout>
            <div class="section w-full mt-16 ">
                <div class="md:flex grid grid-cols-1">
                    <div class="flex-auto md:w-64 w-98 m-9">
                        <img class="w-full h-full rounded-xl"
                            src="https://img.freepik.com/free-photo/tasty-omelette-tomato-slices-white-plate_114579-73850.jpg?w=826&t=st=1683692086~exp=1683692686~hmac=d77dc7bdcf9c03fe1877648fa7847114fae9d176f15c830fdec0cdcd8a7e4fe2"
                            alt="">
                    </div>
                    <div class="flex flex-auto md:w-32 w-98 text-justify items-center px-9">
                        <p class="hover:underline">
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
                            <div v-for="ingredient in ingredients"
                                class="col flex items-center justify-center border p-3 border-black rounded hover:underline">
                                {{ ingredient.items }}
                            </div>
                        </div>
                    </div>
                    <div class="md:flex-auto md:w-64 w-98 m-9 md:mt-9 mt-16 h-80">
                        <h2 class="text-xl font-semibold text-center underline hover:text-lg">Instruction</h2>
                        <div class="card border border-black rounded text-center mt-9 min-h-fit h-full">
                            <div class=" instruction px-6" v-for="step in steps">
                                <h3 class="text-sm py-5 hover:underline">
                                    Step {{ step.numba }}
                                </h3>
                                <p class="h-full text-center hover:underline">
                                    {{ step.text }}
                                </p>
                            </div>
                        </div>
                        <div class="grid grid-cols-2 gap-2">
                            <button class="w3-button w3-black w3-display-left" @click="ganti(-1)">&#10094;</button>
                            <button class="w3-button w3-black w3-display-right" @click="ganti(1)">&#10095;</button>
                        </div>
                    </div>
                </div>
            </div>
            <div class="section video mt-16 mx-auto">
                <h2 class="text-xl font-semibold text-center underline hover:text-lg">Video</h2>
                <iframe class="mt-5 rounded-xl hover:border border-2 border-yellow-500" width="100%" height="315px"
                    src="https://www.youtube.com/embed/y-Wr401Bio4" title="YouTube video player" frameborder="0"
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                    allowfullscreen></iframe>
            </div>
        </div>
        <div class="footer border border-black rounded-xl p-3 mt-10 mb-5 text-center hover:underline m-8">
            <a href="https://www.instagram.com/jaanck_/" target="_blank">
                Create by Fauzan &copy;copyright
            </a>
        </div>
    </div>
</template>

<style>
body {
    @apply font-mono bg-yellow-500;
}

::-webkit-scrollbar {
    @apply w-1
}

::-webkit-scrollbar-thumb {
    @apply bg-yellow-700 rounded mx-2;
}

::-webkit-scrollbar-thumb:hover {
    @apply bg-yellow-950;
}

.instruction {
    @apply block;
}

.card {
    @apply relative block;
}

.video {
    max-width: 680px;
}
</style>

<script>
export default {
    data() {
        return {
            layouts: {
                header: "the-header"
            },
            indexnya: 1,
            steps: [
                { numba: 1, text: "Whisk eggs, water, salt and pepper." },
                {
                    numba: 2, text: `Spray 8-inch (20 cm) non-stick skillet with cooking spray. Heat over medium heat.
                    Pour in egg mixture. As eggs set around edge of skillet, with spatula, gently push
                    cooked portions toward centre of skillet. Tilt and rotate skillet to allow uncooked
                    egg to flow into empty spaces.`},
                {
                    numba: 3, text: `When eggs are almost set on surface but still look moist, cover half of omelette
                        with filling. Slip spatula under unfilled side; fold over onto filled half.`},
                { numba: 4, text: `Cook for a minute, then slide omelette onto plate.` },

            ],
            ingredients: [
                { items: "Eggs" },
                { items: "2" },
                { items: "Salt" },
                { items: "2 tsb (30ml)" },
                { items: "Pepper" },
                { items: "Just A Pinch" },
                { items: "Filling Ingredients" },
                { items: "Just Fill With All u Want" },
            ]
        }
    },
    methods: {
        ganti(n) {
            this.tampil(this.indexnya += n);
            console.log(this.indexnya);
        },
        tampil(n) {
            var i;
            var x = document.getElementsByClassName("instruction");
            if (n > x.length) { this.indexnya = 1 }
            if (n < 1) { this.indexnya = x.length }
            for (i = 0; i < x.length; i++) {
                x[i].style.display = "none";
            }
            x[this.indexnya - 1].style.display = "block";
        }
    },
    mounted() {
        this.tampil(this.indexnya)
    }
}
</script>


