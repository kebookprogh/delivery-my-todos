<script setup lang="ts">
import AtomTitle from '~/components/atoms/atomTitle/atomTitle.vue';

const experts = [{
    id: 1,
    name: 'Spyked',
    image: 'https://kronus.kebook.com.br/assets/79f6dec2-2ac6-48cf-95ac-62b17b60334d/expert-mid.png.webp?format=webp&quality=80',
    path: '/spyked'
},
{
    id: 2,
    name: 'Michel',
    image: 'https://kronus.kebook.com.br/assets/dbdfe559-701c-4fba-8759-b124ffb171ab/expert-mid.png.webp?format=webp&quality=80',
    path: '/michel'
},]
</script>

<template>
    <section class="background flex flex-col items-center justify-center space-x-14 h-[100vh]">
        <h1 class="neon-title mb-10 font-bold text-[#E90218] border-4 border border-[#E90218] rounded-md p-4">Copys dos Experts</h1>
        <div class="flex space-x-14">
            <a v-for="expert in experts" :href="expert.path" :key="expert.id">
                <Avatar class="w-52 h-52 border border-black border-double hover:shadow-2xl shadow-yellow-400 hover:scale-110 duration-200">
                    <AvatarImage class="w-52 h-52" :src="expert.image" alt="expert photo" />
                    <AvatarFallback>KbK</AvatarFallback>
                </Avatar>
            </a>
        </div>
    </section>
</template>

<style scoped>
.background {
    background-image: url(/public/images/background.png);
    background-size: cover;
}

.neon-title:hover {
    color: #fff;
    animation-duration: 200ms;
    transition-duration: 200ms;
    box-shadow: 0 0 15px #E90218, inset 0 0 15px #E90218;
    text-shadow: 0 0 15px #E90218, inset 0 0 15px #E90218!important;
}
</style>