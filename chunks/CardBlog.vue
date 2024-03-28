<template>
    <div class="flex flex-col w-full h-full gap-5">
        <a :href="`/blog/${blogPath}`">
            <img :src="blog.img" alt="" class="max-w-md md:max-w-lg lg:max-w-2xl rounded-lg">
        </a>
        <div class="flex gap-3">
            <div class="flex gap-1">
                <img width="20" height="20" class="flex items-center"
                    src="https://img.icons8.com/material-rounded/24/0000ff/user.png" alt="user" />
                <p class="font-semibold text-sm text-blue-700 flex items-center">{{ blog.user }}</p>
            </div>
            <div class="flex gap-1">
                <img width="22" height="22"
                    src="https://img.icons8.com/external-tanah-basah-basic-outline-tanah-basah/24/0000ff/external-agenda-strategy-tanah-basah-basic-outline-tanah-basah.png"
                    alt="external-agenda-strategy-tanah-basah-basic-outline-tanah-basah" />
                <p class="font-semibold text-sm text-blue-700 flex items-center">{{ blog.timeCreation }}</p>
            </div>
        </div>
        <h6 class='flex items-start text-lg md:text-xl font-bold'>{{ blog.title }}</h6>
        <p class="max-w-md md:max-w-lg lg:max-w-2xl overflow-hidden whitespace-nowrap overflow-ellipsis">{{ blog.discription }}</p>
        <div class="flex gap-2">
            <p class="text-xs md:text-sm underline text-gray-400 " v-for="tag in blog.tags">{{ tag }}</p>
        </div>
    </div>
</template>
<script setup>
const { blog , blogPath  } = defineProps(['blog','blogPath']);
</script>