<template>
    <div id="about" class="container mt-96 pt-40 lg:pt-0 md:pt-20 lg:mt-0 mx-auto flex md:justify-between flex-wrap justify-center gap-11">
        <div class="relative bg-blue-100 flex items-center justify-center flex-col rounded-lg p-20 w-20 h-20 z-0 shadow-lg">
            <img class="w-20 absolute top-1/2 transform -translate-y-1/2" src="/img/book-online.svg" alt="" loading="lazy">
            <p class="font-bold absolute text-blue-700 top-32">Book Online</p>
        </div>
        <div class="relative bg-blue-700 md:-mt-20 flex items-center justify-center rounded-lg p-20 w-20 h-20 z-0 shadow-lg">
            <img class="w-20 absolute top-1/2 transform -translate-y-1/2" src="/img/we-arrive.svg" alt="" loading="lazy">
            <p class="font-bold text-white absolute top-32">We arrive</p>
        </div>
        <div class="relative bg-blue-100 flex items-center justify-center rounded-lg p-20 w-20 h-20 z-0 shadow-lg">
            <img class="w-20 absolute top-1/2 transform -translate-y-1/2" src="/img/slove-problem.svg" alt="" loading="lazy">
            <p class="font-bold absolute text-blue-700 top-32">Slove Problem</p>
        </div>
    </div>
    <section class="container mt-11 flex flex-col md:flex-row mx-auto w-full md:gap-5 lg:gap-10">
        <img src="/img/plumber-about.webp" class="object-cover md:w-1/2  lg:max-w-[45rem] rounded-xl" alt="" loading="lazy">
        <div class="md:w-1/2 flex ml-4 mt-3 md:m-0 flex-col items-start gap-5">
            <p class="font-semibold text-lg relative text-blue-700 flex items-center gap-3"><span class="inline-block  rotate-90 w-[3px] h-[1rem] bg-blue-700"></span>About<span class="inline-block rotate-90 w-[3px] h-[1rem] bg-blue-700"></span></p>
            <h2 class="font-bold md:font-semibold  md:text-xl xl:text-4xl lg:tracking-wide"> Over 18 Years of Expertise in <br/> Manchester Plumbing</h2>
            <p class="max-w-lg text-sm font-semibold">REP offers 24/7 plumbing services in Manchester. Our skilled team ensures prompt, transparent solutions for emergencies and routine tasks. Choose REP for excellence, professionalism, and customer satisfaction, restoring peace of mind efficiently.</p>
            <p class="max-w-lg text-sm font-semibold">With over 18 years of experience, REP is a trusted name in Manchester plumbing. We are dedicated to providing reliable solutions, ensuring your home and plumbing system are in safe hands. Contact us for quick and correct plumbing services.</p>
            <Call></Call>
        </div>
    </section>
</template>
<script setup>
import Call from '/chunks/Call.vue'
</script>