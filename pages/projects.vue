<template>
    <div class="pr-0 lg:pr-48">
        <h1 class='text-primary font-bold text-3xl mb-6'>Projects</h1>

        <div class="grid lg:grid-cols-3 md:grid-cols-2 sm:grid-cols-1 gap-4">
            <ProjectCard
                title="EduQuest"
                description="Gamified web app helping children with learning differences learn through tracing and number-matching games."
                image="/img/projects/eduquest.png"
                link="https://adzu-bluecode.vercel.app/"
                githubRepo="https://github.com/AJ-Orillineda/adzu-bluecode"
                />
            <ProjectCard
                title="NSTP Profiling System for AdZU"
                description="Offline management system for student data with spreadsheet import/export. "
                image="/img/projects/eduquest.png"
                link=""
                githubRepo="https://github.com/janthetrashcan/nstp-profiling-system"
                />
            <ProjectCard
                title="COMTECH School Website"
                description="School website with admissions system for course applications and admin approvals. "
                image="/img/projects/eduquest.png"
                link="https://comtech-site.onrender.com/"
                githubRepo=""
                />
            <ProjectCard
                title="EaglesEye"
                description="Android app featuring an interactive campus map with office locations for students and visitors."
                image="/img/projects/eduquest.png"
                link=""
                githubRepo="https://github.com/janthetrashcan/EaglesEye"
                />
        </div>
    </div>
</template>