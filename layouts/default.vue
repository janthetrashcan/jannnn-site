<template>
    <div class="font-display z-50 bg-primary-bg min-h-screen max-w-screen">
        <div class="flex flex-col sm:flex-row min-h-screen">
            <div class="flex flex-col w-full sm:fixed sm:w-1/5 p-4">
                <Sidebar />
            </div>

            <main class="flex-1 p-8 text-on-primary-bg max-md:mb-32 sm:ml-[20%] overflow-y-auto">
                <slot />
            </main>
        </div>  
    </div>

    <!-- <div id="content-body" class="absolute w-screen h-screen mix-blend-color-dodge hue-rotate-150 opacity-40 z-10"></div> -->
    <!-- <div class="bg-primary-bg absolute w-screen h-screen z-0"></div> -->
</template>

<style scoped>
    #content-body {
        background-image: url('/svg/halftone.jpg');
        background-repeat: no-repeat;
        background-size: 100%;
        background-position: center;
        /* background-position-x: -50%;
        background-position-y: 400%; */
    }
</style>