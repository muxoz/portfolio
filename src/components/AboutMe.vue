<script setup>
import {stack} from "@/data/stack.js";

</script>

<template>
    <header class="grid grid-cols-1 md:grid-cols-2 gap-2 md:my-20 space-y-2">
        <article class="px-10 space-y-3">
            <h1 class="badge badge-success badge-soft text-sm font-extrabold md:text-xl xl:text-3xl  py-5 ">
                $Desarrollador Backend
                <span class="icon-[tabler--brand-laravel] size-10 text-red-600"></span>
            </h1>

            <p class="mt-2  md:text-xl text-slate-300 ">
                Mi nombre es Estiven Muñoz, estudiante de Ingeniería de Sistemas enfocado en el desarrollo backend.
                Tengo experiencia con tecnologías como <span
                    class="px-2 text-red-600 bg-white rounded-md">Laravel</span>,
                <span class="px-2 bg-white rounded-md text-violet-700">Inertia</span> y
                <span class="px-2 bg-white rounded-md text-emerald-500">Vue</span>.
            </p>

            <div class="drawer-content">
                <label for="my-drawer" class="btn btn-success btn-soft btn-block drawer-button">Proyectos</label>
            </div>

            <button class="btn btn-block btn-soft btn-secondary" onclick="my_modal_1.showModal()">Formación</button>


            <a href="./Estiven_Muñoz_CV.pdf" target="_blank" class="btn btn-success btn-soft btn-block">Ver CV</a>


        </article>

        <article class="flex flex-wrap gap-2 justify-center px-4">
            <div class="badge badge-neutral badge-soft w-1/5 h-1/3 transform hover:scale-105 hover:rotate-1 "
                :title="tech.name" v-for="tech, i in stack" :key="i" v-html="tech.span" />
        </article>
    </header>
</template>
