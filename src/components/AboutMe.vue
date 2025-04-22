<script setup>


const stack = [
    {
        name: "Laravel",
        span: '<span class="icon-[tabler--brand-laravel] size-10 text-red-500"></span>'
    },
    {
        name: "MySQL",
        span: '<span class="icon-[tabler--brand-mysql] size-10 text-yellow-500"></span>'
    },
    {
        name: "Inertia.js",
        span: '<span class="icon-[tabler--brand-inertia] size-10 text-violet-500"></span>'
    },
    {
        name: "Vue",
        span: '<span class="icon-[tabler--brand-vue] size-10 text-teal-500"></span>'
    },
    {
        name: "Alpine.js",
        span: '<span class="icon-[tabler--brand-alpine-js] size-10 text-sky-500"></span>'
    },
    {
        name: "TailwindCSS",
        span: '<span class="icon-[tabler--brand-tailwind] size-10 text-sky-500"></span>'
    },
    {
        name: "Bootstrap",
        span: '<span class="icon-[tabler--brand-bootstrap] size-10 text-purple-500"></span>'
    },
    {
        name: "Git",
        span: '<span class="icon-[tabler--brand-git] size-10 text-orange-500"></span>'
    },
    {
        name: "React",
        span: '<span class="icon-[tabler--brand-react] size-10 text-blue-500"></span>'
    },
    {
        name: "PHP",
        span: '<span class="icon-[tabler--brand-php] size-10 text-purple-500"></span>'
    },
    {
        name: "HTML",
        span: '<span class="icon-[tabler--brand-html5] size-10 text-orange-600"></span>'
    },
    {
        name: "CSS",
        span: '<span class="icon-[tabler--brand-css3] size-10 text-sky-600"></span>'
    },
]

</script>

<template>
    <header class="grid grid-cols-1 md:grid-cols-2 gap-2 md:my-20 space-y-2">
        <article class="px-10 space-y-3">
            <h1 class="badge badge-accent badge-soft text-sm font-extrabold md:text-xl xl:text-3xl  py-5 ">
                $Desarrollador Backend
                <span class="icon-[tabler--brand-laravel] size-10 text-red-600"></span>
            </h1>
            
            <p class="mt-2  md:text-xl text-slate-300 ">
                Mi nombre es Estiven Muñoz, estudiante de Ingeniería de Sistemas enfocado en el desarrollo backend. Tengo experiencia con tecnologías como <span class="px-2 text-red-600 bg-white rounded-md">Laravel</span>,
                <span class="px-2 bg-white rounded-md text-violet-700">Inertia</span> y
                <span class="px-2 bg-white rounded-md text-emerald-500">Vue</span>.
            </p>
            <button class="btn btn-gradient btn-success btn-block"  aria-haspopup="dialog"
             aria-expanded="false" aria-controls="overlay-example" data-overlay="#overlay-example"
            >Proyectos</button>

            <button class="btn btn-gradient btn-info btn-block" aria-haspopup="dialog" 
            aria-expanded="false" aria-controls="basic-modal" data-overlay="#basic-modal" 
            >Formación</button>

            <a href="./Estiven_Muñoz_CV.pdf" target="_blank"
            class="btn btn-gradient btn-accent btn-block">Ver CV</a>

           
        </article>

        <article class="flex flex-wrap gap-2 justify-center px-4">
            <div class="badge badge-neutral badge-soft w-1/5 h-1/3 transform hover:scale-105" :title="tech.name"
                v-for="tech, i in stack" :key="i" v-html="tech.span" />
        </article>
    </header>
</template>

