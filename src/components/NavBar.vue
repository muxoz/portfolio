<script setup>
import Email from '@/icons/socials/Email.vue';
import Github from '@/icons/socials/Github.vue';
import Linkedin from '@/icons/socials/Linkedin.vue';
</script>

<template>
    <nav className="container flex flex-col flex-wrap items-center px-3 py-4 mx-auto md:px-0 md:flex-row">
        <button
            className="flex items-center mb-4 font-semibold text-gray-200 transition-opacity duration-200 title-font md:mb-0 hover:opacity-75">
            <img src="/profile.svg" alt="profile"
                className="w-16 h-16 p-2 badge badge-accent badge-soft rounded-full" />
        </button>
        <div
            className="flex flex-wrap items-center justify-around w-full space-x-0 text-base font-normal text-gray-200 md:w-auto md:ml-auto md:space-x-4 lg:justify-center">
            <button class="btn btn-soft btn-accent rounded-full duration-500 hover:scale-95 animate-pulse">
                estivenm0
            </button>

            <a class="btn btn-soft btn-info btn-circle duration-500 hover:scale-95"
                href="https://www.linkedin.com/in/maycolmu%C3%B1oz/" target="_blank" rel="noopener noreferrer">
                <Linkedin />
            </a>
            <a class="btn btn-soft btn-primary btn-circle duration-500 hover:scale-95"
                href="https://github.com/estivenm0" target="_blank" rel="noopener noreferrer">
                <Github />
            </a>

            <a href="mailto:macarny4@gmail.com" class="btn btn-soft btn-error btn-circle duration-500 hover:scale-95">
                <Email />
            </a>
        </div>
    </nav>
</template>
