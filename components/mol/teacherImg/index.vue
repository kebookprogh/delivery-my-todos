<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps<{
    teacherImg: string | undefined
}>()
</script>
<template>
    <section>
        <div>
            <img class="w-96 h-96 object-contain hover:animate-spin hover:delay-300"
                :src="teacherImg"
                alt="teacherImage">
        </div>
    </section>
</template>