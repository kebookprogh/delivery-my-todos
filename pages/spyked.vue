<script setup lang="ts">
import TeacherImg from '@/components/mol/teacherImg/index.vue'
import CarouselSpy from '@/components/organism/carouselSpy/index.vue'

</script>

<template>
    <section class="background flex items-center justify-center space-x-14 h-[100vh]">
        <TeacherImg :teacherImg="'https://kronus.kebook.com.br/assets/a37d7977-faf8-46e2-be95-5cae3c98b7d7/expert-top.png.webp?format=webp&quality=80'"/>
        <CarouselSpy />
        <TeacherImg :teacherImg="'https://kronus.kebook.com.br/assets/a37d7977-faf8-46e2-be95-5cae3c98b7d7/expert-top.png.webp?format=webp&quality=80'"/>
    </section>
</template>

<style scoped>
.background {
    background-image: url(https://kronus.kebook.com.br/assets/e5353a36-0efe-4d29-96d8-9642669c89e8/back-content-b.png.webp);
}
</style>