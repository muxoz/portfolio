<script setup lang="ts">
import { education } from '@/data/education.js';
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
</script>

<template>
  <Dialog>
    <DialogTrigger as-child>
      <Button variant="outline" class="w-full"> Formación </Button>
    </DialogTrigger>
    <DialogContent class="max-h-[90dvh] grid-rows-[auto_minmax(0,1fr)_auto] p-0 sm:max-w-[425px]">
      <DialogHeader class="p-6 pb-0">
        <DialogTitle>Formación</DialogTitle>
      </DialogHeader>
      <div class="grid gap-4 overflow-y-auto px-6 py-4">
        <div class="flex flex-col justify-between">
          <Accordion type="single" collapsible>
            <template v-for="item in education" :key="i">
              <AccordionItem :value="item.title">
                <AccordionTrigger> {{ item.title }} </AccordionTrigger>
                <AccordionContent> {{ item.description }} </AccordionContent>
              </AccordionItem>
            </template>
          </Accordion>
        </div>
      </div>
    </DialogContent>
  </Dialog>
</template>
