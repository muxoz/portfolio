<script setup>
import { stack } from '@/data/stack.js';
import Badge from './ui/badge/Badge.vue';
import Button from './ui/button/Button.vue';
import MyEducation from './MyEducation.vue';
import MyProjects from './MyProjects.vue';
</script>

<template>
  <header class="grid grid-cols-1 gap-2 space-y-2 md:my-20 md:grid-cols-2">
    <article class="space-y-3 px-10">
      <h1>
        <Badge class="py-2 text-sm font-extrabold md:text-xl"> $ Desarrollador Backend </Badge>
      </h1>

      <p class="mt-2 text-slate-300 md:text-xl">
        Mi nombre es Maycol Muñoz, estudiante de Ingeniería de Sistemas enfocado en el desarrollo
        backend. Tengo experiencia con tecnologías como
        <span class="rounded-md bg-white px-2 text-red-600">Laravel</span>,
        <span class="rounded-md bg-white px-2 text-pink-600">livewire</span>,
        <span class="rounded-md bg-white px-2 text-violet-700">Inertia</span> y
        <span class="rounded-md bg-white px-2 text-emerald-500">Vue</span>.
      </p>

      <MyProjects />

      <MyEducation />

      <Button class="w-full" variant="outline" as="a" target="_blank" href="./Maycol_Muñoz_CV.pdf">
        Ver CV
      </Button>
    </article>

    <article class="flex flex-wrap justify-center gap-2 px-4">
      <div
        class="flex w-1/5 transform justify-center rounded-2xl bg-white/5 p-0 hover:rotate-1 hover:scale-105"
        :title="tech.name"
        v-for="(tech, i) in stack"
        :key="i"
        v-html="tech.span"
      ></div>
    </article>
  </header>
</template>
