<template>
    <NuxtLayout :name="layouts.header">
        <div class="section w-full" id="destinasi">
            <div class="text-center mx-16">
                <Navbar />
            </div>
        </div>
    </NuxtLayout>
    
    <div class="section w-full" id="destinasi">
        <div class="my-20 text-center mx-16">
            <Destination>

            </Destination>
        </div>
    </div>
    <div class="section w-full" id="blog">
        <div class="my-10 text-center mx-16">
            <Blog>
            </Blog>
        </div>
    </div>
    <div class="section w-full" id="blog">
        <div class="my-10 text-center mx-16">
            <Blog2>
            </Blog2>
        </div>
    </div>

    <NuxtLayout :name="layouts.footer" />
</template>
<style>
body {
    @apply font-sans;
}
</style>
<script>
export default {
    data() {
        return {
            layouts: {
                navbar: "navbar",
                header: "header",
                footer: "footer"
            },
            cardData: {
                text: `Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nam, animi! Iure necessitatibus eaque error ducimus corporis cupiditate doloribus totam? Unde necessitatibus corrupti, laudantium esse assumenda, mollitia pariatur praesentium quam itaque corporis repudiandae similique aliquam. Odio exercitationem accusantium eius sunt vitae quia consequuntur nemo, iusto, labore numquam sapiente quibusdam officia suscipit at. Facilis consequuntur explicabo ipsum porro quibusdam nulla fugit culpa, reiciendis, voluptas expedita a exercitationem natus sint delectus doloribus dolore veritatis saepe repellendus voluptatibus libero aperiam! Nulla, rem? Placeat beatae, hic neque repudiandae vero quis, doloremque expedita aliquam error odio dicta in quidem nisi dolorum iusto quas ullam, sit voluptas!F`,
                image: "/img/coming-soon.avif"
            },
            sectionData: {

            }
        }
    }
}
</script>