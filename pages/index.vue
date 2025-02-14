<script setup lang="ts">
import {
    Carousel,
    CarouselContent,
    CarouselItem,
    CarouselNext,
    CarouselPrevious,
} from '@/components/atoms/ui/carousel'
import TeacherImg from '@/components/mol/teacherImg/index.vue'

const entregas = [
    {
        id: 1,
        thumb: "https://kronus.kebook.com.br/assets/8926ea06-fcf6-47c0-9c3a-440c1a3478a6/content-expert.png",
        archive: "1e5uXSRLgVVLzNyM8MYxwQ3zAK-4wU_wp"
    },
    {
        id: 2,
        thumb: "https://kronus.kebook.com.br/assets/5ceb4048-d058-4be9-9622-202c8069e405/content-expert.png",
        archive: "1QoneeHc46b5IIJdONy9b0Wgt0KK2OOwN"
    },
    {
        id: 3,
        thumb: "https://kronus.kebook.com.br/assets/55bc81e1-d7c7-4867-a32c-90913c64962d/content-expert.png",
        archive: "19U2z9Eg7GlB4PhPA58oaFEfTYJNZJrSs"
    },
    {
        id: 4,
        thumb: "https://kronus.kebook.com.br/assets/82f99475-cd26-4050-afc5-ab08a5161227/content-expert.png",
        archive: "1K0r7TvlwLLrZNVF6v7o39RRj_33aT48X"
    },
    {
        id: 5,
        thumb: "https://kronus.kebook.com.br/assets/55c25079-1155-4fbc-8cb9-7d950a7f5b7d/content-expert.png",
        archive: "1cyj7YoRYqHVdLcmWVjToyvoadcBlAF-y"
    },
    {
        id: 6,
        thumb: "https://kronus.kebook.com.br/assets/cdcb5c8d-24ba-4783-bb99-99fa0264b07d/content-expert.png",
        archive: "1xmy_gz4LFdQkBM1J_-RSH7Ob21aWJfln"
    }

]
</script>

<template>
    <section class="background flex items-center justify-center space-x-14 h-[100vh]">
        <TeacherImg />
        <section class="flex flex-col items-center justify-center mt-10">
            <h1 class="text-4xl font-bold mt-[-200px] mb-28">Copys do Spyked</h1>
            <div class="w-64 h-64 ">
                <Carousel>
                    <CarouselContent>
                        <CarouselItem v-for="delivery in entregas" :key="delivery.id" class="flex flex-col hover:animate-pulse">
                            <img class="object-cover h-56"
                                :src="delivery.thumb"
                                alt="">
                            <a :href="`https://drive.google.com/uc?export=download&id=${ delivery.archive }`">
                                <button
                                    class="bg-yellow-500 w-full font-black rounded-b-lg p-2 hover:bg-yellow-600 hover:delay-200">Clica
                                    em mim!</button></a>
                        </CarouselItem>
                    </CarouselContent>
                    <CarouselPrevious />
                    <CarouselNext />
                </Carousel>
            </div>
        </section>
        <TeacherImg />
    </section>
</template>

<style scoped>
.background {
    background-image: url(https://kronus.kebook.com.br/assets/e5353a36-0efe-4d29-96d8-9642669c89e8/back-content-b.png.webp);
}
</style>