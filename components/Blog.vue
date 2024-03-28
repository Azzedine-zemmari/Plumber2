<template>
<div class="md:-mt-10  relative w-full min-h-[400px]">
<img src="/img/blog-hero.webp" alt="" class="object-cover w-full min-h-[400px]">
<div class="w-full h-full absolute inset-0 bg-blue-600 opacity-70"></div>
<h1 class="font-bold text-3xl sm:text-5xl text-white absolute -translate-x-1/2 -translate-y-1/2 z-40 top-1/2 left-1/2"> REP - Blog  </h1>
</div>
<template class=" mx-auto" v-for="blog in blogS">
    <div class=" grid place-content-center my-7 ">
        <CardB :blog="blog" :blogPath="blog.id" />   
    </div>
</template>
</template> 
<script setup>
import {blogS} from "/data.js"
import CardB from "/chunks/CardBlog.vue"
</script>