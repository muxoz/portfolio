<script setup>
import Email from '@/icons/socials/Email.vue';
import Github from '@/icons/socials/Github.vue';
import Linkedin from '@/icons/socials/Linkedin.vue';

import { Button } from '@/components/ui/button';
</script>

<template>
  <nav
    className="container flex flex-col flex-wrap items-center px-3 py-4 mx-auto md:px-0 md:flex-row"
  >
    <Button class="rounded-4xl p-1">
      <img
        src="/profile.svg"
        alt="profile"
        className="w-16 h-16 p-2 badge badge-accent badge-soft rounded-full"
      />
    </Button>
    <div
      className="flex flex-wrap items-center justify-around w-full space-x-0 text-base font-normal text-gray-200 md:w-auto md:ml-auto md:space-x-4 lg:justify-center mt-2"
    >
      <button
        class="btn btn-soft btn-accent animate-pulse rounded-full duration-500 hover:scale-95"
      >
        Muxzz
      </button>

      <a
        class="btn btn-soft btn-info btn-circle duration-500 hover:scale-95"
        href="https://www.linkedin.com/in/maycolmu%C3%B1oz/"
        target="_blank"
        rel="noopener noreferrer"
      >
        <Linkedin />
      </a>
      <a
        class="btn btn-soft btn-primary btn-circle duration-500 hover:scale-95"
        href="https://github.com/muxzz"
        target="_blank"
        rel="noopener noreferrer"
      >
        <Github />
      </a>

      <a
        href="mailto:macarny4@gmail.com"
        class="btn btn-soft btn-error btn-circle duration-500 hover:scale-95"
      >
        <Email />
      </a>
    </div>
  </nav>
</template>
