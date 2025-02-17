<script setup lang="ts">
import CarouselExcel from '@/components/organism/carouselExcel/index.vue'
import TeacherImg from '@/components/mol/teacherImg/index.vue'
</script>

<template>
    <section class="background flex items-center justify-center space-x-14 h-[100vh]">
        <TeacherImg />
        <CarouselExcel />
        <TeacherImg />
    </section>
</template>

<style scoped>
.background {
    background-image: url(https://kronus.kebook.com.br/assets/3df83d07-dd61-4b9d-aa1e-173a76233df6/back-content-b.png.webp);
}
</style>