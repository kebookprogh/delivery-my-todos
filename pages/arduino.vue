<script setup lang="ts">
import TeacherImg from '@/components/mol/teacherImg/index.vue'
import CarouselArdu from '@/components/organism/carouselArdu/index.vue'

</script>

<template>
    <section class="background flex items-center justify-center space-x-14 h-[100vh]">
        <TeacherImg :teacherImg="'https://kronus.kebook.com.br/assets/6bf14529-ba27-4726-b0ec-a9149a96051e/expert-top.png.webp?format=webp&quality=80'"/>
        <CarouselArdu />
        <TeacherImg :teacherImg="'https://kronus.kebook.com.br/assets/6bf14529-ba27-4726-b0ec-a9149a96051e/expert-top.png.webp?format=webp&quality=80'"/>
    </section>
</template>

<style scoped>
.background {
    background-image: url(https://kronus.kebook.com.br/assets/4263e51d-c53a-48bf-848e-ccdb1ed5455c/back-top-w.png);
    background-size: cover;
}
</style>