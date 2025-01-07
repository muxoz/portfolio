<script setup>
import projects from "@/data/projects.json";
</script>

<template>
    <div id="overlay-example" class="overlay overlay-open:translate-x-0 drawer drawer-start hidden" role="dialog"
    tabindex="-1">
    <div class="drawer-header">
      <h3 class="drawer-title">PROYECTOS</h3>
      <button type="button" class="btn btn-text btn-circle btn-sm absolute end-3 top-3" aria-label="Close"
        data-overlay="#overlay-example">
        <span class="icon-[tabler--x] size-5"></span>
      </button>
    </div>
    <div class="drawer-body">
      <p>
      <div class="accordion accordion-bordered">
        <template v-for="project, i in projects" :key="i">

          <div class="accordion-item" :id="i">
            <button class="accordion-toggle inline-flex items-center gap-x-4 px-5 py-4 text-start" :aria-controls="i"
              :aria-expanded="false">
              <span
                class="icon-[tabler--plus] accordion-item-active:hidden text-base-content size-4.5 block shrink-0"></span>
              <span
                class="icon-[tabler--minus] accordion-item-active:block text-base-content size-4.5 hidden shrink-0"></span>
              {{ project.title }}
            </button>
            <div :id="i" class="accordion-content hidden w-full overflow-hidden transition-[height] duration-300"
              :aria-labelledby="i" :role="i">
              <div class="px-5 pb-4">
                <img :src="project.img" alt="">
                <template v-for="tech, i in project.stack" :key="i">
                  <span class="badge badge-soft badge-info m-1 " >{{ tech }}</span>
                </template>
                <p class="text-base-content/80 font-normal">
                  {{ project.description }}
                </p>
                <a :href="project.repository" target="_blank" class="btn btn-gradient btn-secondary btn-block">
                    Repositorio
                    <span class="icon-[tabler--brand-github]"></span>
                </a>
              </div>
            </div>
          </div>
        </template>

      </div>




      </p>
    </div>
    <div class="drawer-footer">
      <button type="button" class="btn btn-soft btn-accent" data-overlay="#overlay-example">Cerrar</button>
    </div>
  </div>
</template>

