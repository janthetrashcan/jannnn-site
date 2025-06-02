<script setup>

const props = defineProps({
    class: {
        type: String,
        default: '',
        required: false
    },
})

</script>

<template>
    <header
    :class=props.class
    class="flex h-fit py-6 w-full items-center justify-center">
        <NuxtImg
        src="/img/logo-white.png"
        alt="Logo"
        class="object-cover h-10 w-fit"
        />
    </header>
</template>