<script setup>


</script>

<template>
    <div class="bg-gray-900 p-6 rounded-lg shadow-md container mx-auto w-3/4 text-center">
    <h2 class="text-3xl font-semibold text-white mb-4">Subscribe to Our Blog</h2>
    <p class="text-gray-300 mb-4">Stay updated with our latest blog posts by subscribing to our newsletter.</p>
    <form class="flex flex-col">
        <label for="email" class="text-gray-400 mb-2">Email Address</label>
        <input type="email" id="email" name="email" placeholder="you@example.com" class="border bg-gray-800 rounded-lg py-2 px-3 focus:outline-none focus:ring-2 focus:ring-blue-300 mb-4 text-white">
        <button type="submit" class="font-bold bg-rose-500 hover:bg-rose-600 transition duration-300 text-white rounded-lg py-2">
            Subscribe
        </button>
    </form>
</div>


</template>