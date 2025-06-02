<template>
    <div class="font-display z-50 bg-primary-bg min-h-screen max-w-screen no-scrollbar">
        <div class="flex flex-col sm:flex-row min-h-screen">
            <div class="bg-primary-bg flex flex-col w-full fixed bottom-0 sm:fixed sm:top-0 sm:w-1/6 z-50 p-4">
                <Sidebar />
            </div>

            <div class="fixed sm:hidden bg-primary-bg top-0 left-0 w-full z-50">  
                <Header />
            </div>

            <main class="flex-1 p-8 text-on-primary-bg max-sm:mt-[12%] max-md:mb-32 sm:ml-[18%] overflow-y-auto">
                <slot />
            </main>
        </div>  
    </div>
</template>