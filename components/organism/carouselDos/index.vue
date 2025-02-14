<script setup lang="ts">
import {
    Carousel,
    CarouselContent,
    CarouselItem,
    CarouselNext,
    CarouselPrevious,
} from '@/components/atoms/ui/carousel'

const entregas = [
    {
        id: 1,
        thumb: "https://kronus.kebook.com.br/assets/8926ea06-fcf6-47c0-9c3a-440c1a3478a6/content-expert.png",
        archive: "1dpm-5fsVt0hRNwtjlBVHGJFkndZ_Jv3a"
    },
    {
        id: 2,
        thumb: "https://kronus.kebook.com.br/assets/5ceb4048-d058-4be9-9622-202c8069e405/content-expert.png",
        archive: "1mPr3qzMEiJ4Rmhtjqmw-LPS1rc0D0jby"
    },
    {
        id: 3,
        thumb: "https://kronus.kebook.com.br/assets/55bc81e1-d7c7-4867-a32c-90913c64962d/content-expert.png",
        archive: "1Nr_LgtSa-P2M9d2rh6iUpsRukA37WscY"
    },
    {
        id: 4,
        thumb: "https://kronus.kebook.com.br/assets/55c25079-1155-4fbc-8cb9-7d950a7f5b7d/content-expert.png",
        archive: "1-X1EVRW8sjNk9hFohLDNoyNBmSGTilOR"
    },
    {
        id: 5,
        thumb: "https://kronus.kebook.com.br/assets/cdcb5c8d-24ba-4783-bb99-99fa0264b07d/content-expert.png",
        archive: "12zbiXZOxzVLXSMsuqy1_tJK1UJSivsWJ"
    }
]
</script>
<template>
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
                                    class="bg-yellow-500 w-full font-black rounded-b-lg p-2 hover:bg-yellow-600 hover:delay-200">Clica em mim!</button></a>
                        </CarouselItem>
                    </CarouselContent>
                    <CarouselPrevious />
                    <CarouselNext />
                </Carousel>
            </div>
        </section>
</template>