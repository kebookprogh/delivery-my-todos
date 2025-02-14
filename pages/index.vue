<script setup lang="ts">
import CarouselSpy from '@/components/organism/carouselSpy/index.vue'
import TeacherImg from '@/components/mol/teacherImg/index.vue'
</script>

<template>
    <section class="background flex items-center justify-center space-x-14 h-[100vh]">
        <TeacherImg />
        <CarouselSpy />
        <TeacherImg />
    </section>
</template>

<style scoped>
.background {
    background-image: url(https://kronus.kebook.com.br/assets/e5353a36-0efe-4d29-96d8-9642669c89e8/back-content-b.png.webp);
}
</style>