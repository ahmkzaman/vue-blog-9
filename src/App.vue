<script setup>
import Nav from './components/views/Nav.vue';
import PostList from './components/views/PostList.vue';
import Footer from './components/views/Footer.vue';
</script>

<template>
  <div class="container mx-auto mt-4 flex justify-between border-2 p-4 rounded-lg">
    <div>
      <h1 class="text-xl font-bold text-rose-700">KZ BLOG</h1>
    </div>
    <div>
      <Nav/>
    </div>
    
  </div>
  <div class="mb-6">
    <PostList/>
  </div>
  <div class="mt-2">
    <Footer/>
  </div>
</template>

<style scoped>

</style>
