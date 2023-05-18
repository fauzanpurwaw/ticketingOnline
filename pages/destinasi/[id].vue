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
            <CardSection :title="id" :image="'/img/' + id + '.webp'">
            </CardSection>
        </div>
    </div>

    <NuxtLayout :name="layouts.footer" />
</template>

<script setup>
const { id } = useRoute().params;
</script>   

<script>
export default {
    data() {
        return {  
            layouts: {
                header: "header",
                footer: "footer"
            },  
            cardData: {
                text: `Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nam, animi! Iure necessitatibus eaque error ducimus corporis cupiditate doloribus totam? Unde necessitatibus corrupti, laudantium esse assumenda, mollitia pariatur praesentium quam itaque corporis repudiandae similique aliquam. Odio exercitationem accusantium eius sunt vitae quia consequuntur nemo, iusto, labore numquam sapiente quibusdam officia suscipit at. Facilis consequuntur explicabo ipsum porro quibusdam nulla fugit culpa, reiciendis, voluptas expedita a exercitationem natus sint delectus doloribus dolore veritatis saepe repellendus voluptatibus libero aperiam! Nulla, rem? Placeat beatae, hic neque repudiandae vero quis, doloremque expedita aliquam error odio dicta in quidem nisi dolorum iusto quas ullam, sit voluptas!F`,
            }
        }
    }
}
</script>