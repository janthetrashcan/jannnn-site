<script setup>

const props = defineProps({
    title: {
        type: String,
        default: 'title',
        required: true
    },
    description: {
        type: String,
        default: '',
        required: true
    },
    link: {
        type: String,
        default: '',
        required: true
    },
    githubRepo: {
        type: String,
        default: '',
        required: false
    },
    image: {
        type: String,
        default: '',
        required: true
    },
    class: {
        type: String,
        default: '',
        required: false
    }
})

</script>

<template>
    <div class="flex flex-col w-full items-start justify-between border-2 border-on-primary-bg/20 rounded-2xl overflow-hidden">
        <NuxtImg :src="props.image" class="object-cover w-full h-48 rounded-lg mb-4" fit="cover" />
       
        <div class="flex flex-col px-4 pt-4 gap-1">
            <h class="text-primary text-2xl font-bold">{{ props.title }}</h>
            <p class="text-on-primary-bg text-lg">{{ props.description }}</p>
        </div>

        <div class="flex flex-row justify-start items-center gap-2 px-4 mb-4 mt-2 w-full h-fit">
            <NuxtLink v-if="props.link"
                class="bg-none text-on-primary-bg w-fit h-8 p-2 flex items-center justify-center rounded-lg hover:bg-primary/20 transition duration-300"
                :to="props.link" target="_blank">
                <Icon name="mingcute:external-link-line" class="text-2xl" />
            </NuxtLink>

            <NuxtLink v-if="props.githubRepo"
                class="bg-none text-on-primary-bg w-fit h-8 p-2 flex items-center justify-center rounded-lg hover:bg-primary/20 transition duration-300"
                :to="props.githubRepo" target="_blank">
                <Icon name="mingcute:github-line" class="text-2xl" />
            </NuxtLink>
        </div>
    </div>
</template>