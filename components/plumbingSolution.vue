<template >
    <section id="Services" class="  w-full  mt-10 pb-20  bg-blue-50 ">
        <div class="flex flex-col items-center justify-center text-center pt-12 md:pt-32">
            <h3 class="font-bold pb-4 text-xl xl:text-4xl">Excellence in Plumbing Solutions</h3>
            <p class="text-sm font-semibold max-w-md md:max-w-2xl">Elevate your plumbing experience in Manchester with
                our
                unmatched precision and excellence. Our</p>
            <p class="text-sm font-semibold max-w-md md:max-w-2xl">reliable, efficient services are tailored to your
                satisfaction, delivering superior solutions.</p>
        </div>
        <div class="container mx-auto grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-2 sm:gap-x-1 sm:gap-y-1">
            <template v-for="(solution, index) in solutions" :key="index">
                <div class="flex justify-center">
                    <Card :blog="solution"></Card>
                </div>
            </template>
        </div>
    </section>
</template>
<script setup>
import { solutions } from '/data.js'
import Card from '/chunks/Card.vue'
</script>