<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps<{
    title: string
}>()
</script>
<template>
<h1 class="text-4xl font-bold mt-[-200px] mb-28">{{ title }}</h1>
</template>