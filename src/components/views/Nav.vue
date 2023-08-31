<script setup>
import { ref } from 'vue'
import axios from 'axios';

let navData = ref([])

getData()
async function getData() {
    let response = await axios.get("https://basic-blog.teamrabbil.com/api/post-categories")
    navData.value = response.data
}

</script>

<template>
   
    <div class="flex justify-end"> 
    <div v-for="nav in navData" :key="nav.id" class="px-4"> 
        <h2 class="text-xl font-bold text-gray-500 hover:text-red-500"> <a href="">{{nav.name}}</a></h2>

    </div>

    </div>
</template>