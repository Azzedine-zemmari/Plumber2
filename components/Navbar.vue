<template>
    <nav class="container bg-white w-full flex justify-between items-center mx-auto p-5">
        <div class="hidden md:flex  items-center gap-3 ">
            <img src="/img/logo.svg" class="w-10" alt="" loading="lazy" />
            <p class="font-semibold text-[20px]">Radiant Emergency Plumber</p>
        </div>
        <div>
            <ul class="hidden md:flex items-center gap-4 lg:gap-10">
                <li class=" font-medium text-lg" v-for="(item, index) in nav" :key="index">
                    <a :href="item.href">{{ item.name }}</a>
                </li>
                <Call></Call>
            </ul>
        </div>
    </nav>
    <nav class=" relative md:mt-10 container bg-white  flex justify-between mx-auto items-center  p-5 -mt-10">
        <div class="flex md:hidden gap-3 items-center">
            <img src="/img/logo.svg" class="w-9" alt="" loading="lazy" />
            <p class="font-semibold text-lg">REP</p>
        </div>
        <button @click="openMenu">
            <img class="flex md:hidden"  width="30" height="30" src="https://img.icons8.com/ios/50/menu--v4.png" alt="menu--v4" loading="lazy" />
        </button>
        <ul v-if="menu" class="absolute z-10 top-20 right-5 flex flex-col px-5 py-3 bg-sky-50 rounded-lg md:hidden justify-start items-start gap-4">
            <li class="font-medium text-lg" v-for="(item, index) in nav" :key="index">
                <a :href="item.href">{{ item.name }}</a>
            </li>
            <Call></Call>
        </ul>
    </nav>
</template>
<script setup>
import {ref} from 'vue'
import { nav } from '/data.js'
import Call from '/chunks/Call.vue'
const menu = ref(false) ;
function openMenu() {
    menu.value = !menu.value;
}
</script>
