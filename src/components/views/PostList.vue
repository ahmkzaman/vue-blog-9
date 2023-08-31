<script setup>
import axios from 'axios'
import { ref } from 'vue'

const postData = ref([])

getData()
async function getData() {
    const response = await axios.get("https://basic-blog.teamrabbil.com/api/post-newest")
    postData.value = response.data
}


</script>

<template>
    
    <div v-for="post in postData" :key="post.id" class="container mx-auto mt-10 w-3/4">
        <img :src="post.img" class="w-full rounded-lg h-2/3" alt="">
        <h1 class="text-xl font-bold mt-6 pl-2">{{post.title}}</h1>
        <h1 class="text-xl mt-4 pl-2">{{post.short}}</h1>
              
    </div>
    
</template>

