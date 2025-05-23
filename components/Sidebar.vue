<template>
    <nav id='navigation' class='flex flex-row sm:flex-col w-full h-full items-center md:items-start gap-1'>
        <NuxtImg
        src="/img/logo-white.png"
        alt="Logo"
        class="hidden sm:block w-16 object-cover mb-0 sm:mb-8 mt-8 ml-4 mr-8 sm:mr-0"
        />

        <NavigationButton label="Home" to="/" iconDefault="mingcute:home-2-line" iconSelected="mingcute:home-2-fill" />
        <NavigationButton label="About" to="/about" iconDefault="mingcute:profile-line" iconSelected="mingcute:profile-fill" />
        <NavigationButton label="Projects" to="/projects" iconDefault="mingcute:documents-line" iconSelected="mingcute:documents-fill" />
        <NavigationButton label="Contact" to="/contact" iconDefault="mingcute:contacts-4-line" iconSelected="mingcute:contacts-4-fill" />
    </nav>
</template>