<script setup>


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
                estivenm
            </button>

            <a href="https://www.linkedin.com/in/maycolmu%C3%B1oz/" target="_blank" rel="noopener noreferrer"
                class="btn btn-circle border-[#0a66c2] bg-[#0a66c2] text-white shadow-[#0a66c2]/30 hover:border-[#0a66c2] hover:bg-[#0a66c2]/90"
                aria-label="Linkedin Icon Button">
                <span class="icon-[tabler--brand-linkedin]"></span>
            </a>
            <a href="https://github.com/estivenm0" target="_blank" rel="noopener noreferrer"
                class="btn btn-circle border-[#2b3137] bg-[#2b3137] text-white shadow-[#2b3137]/30 hover:border-[#2b3137] hover:bg-[#2b3137]/90"
                aria-label="Github Icon Button">
                <span class="icon-[tabler--brand-github]"></span>
            </a>


            <a href="mailto:macarny4@gmail.com" class="btn btn-soft btn-info rounded-full duration-500 hover:scale-95">
                <span class="icon-[tabler--brand-gmail]"></span>
            </a>
        </div>
    </nav>
</template>
