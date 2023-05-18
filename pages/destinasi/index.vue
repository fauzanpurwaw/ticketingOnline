<template>
    <NuxtLayout :name="layouts.header">
        <div class="section w-full" >
            <div class="text-center mx-16">
                <Navbar />
            </div>
        </div>
    </NuxtLayout>
    <div class="section w-full xl:flex xl:justify-center" >
        <div class="my-20 text-center lg:mx-16 sm:mx-10 max-w-7xl" >
            <CardSection :title="title" :image="'/img/' + soon">
                
            </CardSection>
        </div>
    </div>

    <NuxtLayout :name="layouts.footer" />
</template>

<script>
    export default {
    data() {
        return {
            layouts: {
                navbar: "navbar",
                header: "header",
                footer: "footer"
            },
            soon: "coming-soon.avif",
            title: "Coming Soon"
        }
    }
}
</script>