<script setup>

const props = defineProps({
    title: {
        type: String,
        default: 'title',
        required: true
    },
    body: {
        type: String,
        default: '',
        required: true
    },
})

</script>

<template>
    <div class="flex flex-col">
        <h2 class='text-primary font-bold text-xl'>{{ props.title }}</h2>
        <p class='text-on-primary-bg text-lg mb-4'>{{ props.body }}</p>
    </div>
</template>