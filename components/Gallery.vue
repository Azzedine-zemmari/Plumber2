<template>
    <div class="flex flex-col  gap-2  justify-center text-center pt-20">
        <h4 class="font-bold text-xl lg:text-4xl">Plumbing Gallery</h4>
        <p class="semi-bold text-lg lg:text-2xl">Explore our range of plumbing services through the following images.</p>
    </div>
    <div class="container mx-auto mt-10 grid grid-cols-2 md:grid-cols-4  lg:gap-1">
        <template v-for="(row, rowIndex) in gallery" :key="rowIndex">
            <div class="grid gap-2 px-2 ">
                <template v-for="(item, itemIndex) in row" :key="itemIndex">
                    <div class="overflow-hidden mx-auto flex justify-center">
                        <img class="h-auto max-w-full  rounded-lg transition duration-300 ease-in-out hover:scale-110 " :src="item" alt="" loading="lazy">
                    </div>
                </template>
            </div>
        </template>
    </div>
</template>

<script setup>
import { gallery } from '/data.js'
</script>