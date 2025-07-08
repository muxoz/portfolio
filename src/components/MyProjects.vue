<script setup>
import { projects } from "@/data/projects.js";
import Github from "@/icons/socials/Github.vue";
import Link from "@/icons/socials/Link.vue";
</script>

<template>
  <div class="drawer">
    <input id="my-drawer" type="checkbox" class="drawer-toggle" />

    <div class="drawer-side">
      <label for="my-drawer" aria-label="close sidebar" class="drawer-overlay"></label>
      <ul class="menu bg-base-200 text-base-content min-h-full w-80 md:w-96 p-2">
        <template v-for="project, i in projects" :key="i">
          <div class="collapse collapse-plus bg-base-100 border border-base-300">
            <input type="radio" name="my-accordion-3" />
            <div class="collapse-title font-semibold">
              {{ project.title }}
            </div>
            <div class="collapse-content text-sm">
              <img :src="project.img" alt="">
              <template v-for="tech, i in project.stack" :key="i">
                <span class="badge badge-soft badge-info m-1 ">{{ tech }}</span>
              </template>
              <br>

              {{ project.description }}

              <div class="grid grid-cols-2 gap-1 mt-2">
                <a :href="project.repository" target="_blank" title="Repositorio"
                  class="btn btn-soft btn-secondary btn-block">
                  <Github />
                </a>
                <a :href="project.link" target="_blank" title="Vídeo" class="btn btn-soft btn-error btn-block">
                  <Link />
                </a>
              </div>

            </div>
          </div>
        </template>
      </ul>
    </div>
  </div>

</template>
