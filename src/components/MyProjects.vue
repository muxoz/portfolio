<script setup lang="ts">
import { projects } from '@/data/projects.js';
import Github from '@/icons/socials/Github.vue';
import Link from '@/icons/socials/Link.vue';
import { Button } from '@/components/ui/button';
import {
  Accordion,
  AccordionContent,
  AccordionItem,
  AccordionTrigger,
} from '@/components/ui/accordion';
import {
  Dialog,
  DialogContent,
  DialogHeader,
  DialogTitle,
  DialogTrigger,
} from '@/components/ui/dialog';
import Badge from './ui/badge/Badge.vue';
</script>

<template>
  <Dialog>
    <DialogTrigger as-child>
      <Button variant="outline" class="w-full"> Proyectos </Button>
    </DialogTrigger>
    <DialogContent class="max-h-[90dvh] grid-rows-[auto_minmax(0,1fr)_auto] p-0 sm:max-w-[425px]">
      <DialogHeader class="p-6 pb-0">
        <DialogTitle>Proyectos</DialogTitle>
      </DialogHeader>
      <div class="grid gap-4 overflow-y-auto px-6 py-4">
        <div class="flex flex-col justify-between">
          <Accordion type="single" collapsible>
            <template v-for="(project, i) in projects" :key="i">
              <AccordionItem :value="project.title">
                <AccordionTrigger> {{ project.title }}</AccordionTrigger>
                <AccordionContent>

                  <img :src="project.img" alt="" />

                  <template v-for="(tech, i) in project.stack" :key="i">
                    <Badge class="my-1"> {{ tech }} </Badge>
                  </template>
                  
                  <br />

                  {{ project.description }}

                  <div class="mt-2 grid grid-cols-2 gap-1">
                    <Button as="a" :href="project.repository" variant="outline" target="_blank" title="Repositorio">
                      <Github />
                    </Button>
                    <Button as="a" :href="project.link" variant="outline" target="_blank" title="Demo">
                      <Link />
                    </Button>
                  </div>
                </AccordionContent>
              </AccordionItem>
            </template>
          </Accordion>
        </div>
      </div>
    </DialogContent>
  </Dialog>
</template>
