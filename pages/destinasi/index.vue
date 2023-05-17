<template>
    <NuxtLayout :name="layouts.header">
        <Navbar />
    </NuxtLayout>
    <div class="section w-full" id="destinasi">
        <div class="my-5 text-center mx-16">
            <CardSection>
                
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
        }
    }
}
</script>