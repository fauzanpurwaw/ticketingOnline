<template>
    <NuxtLayout :name="layouts.header">
        <Navbar />
    </NuxtLayout>
    <div class="section w-full" id="destinasi">
        <div class="my-5 text-center mx-16">
            <CardSection :title="id" :image="'/img/' + id + '.webp'" :text="cardData.text">
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