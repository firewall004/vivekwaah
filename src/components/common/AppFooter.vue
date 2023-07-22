<template>
  <footer class="bg-zinc-900 mt-auto bottom-0 w-full select-none">
    <div class="mx-auto max-w-7xl overflow-hidden px-6 py-6 lg:px-8">
      <div class="mt-10 flex justify-center space-x-10">
        <social-links />
      </div>
      <p class="mt-10 text-center text-xs leading-5 text-gray-500">
        &copy; 2023 All rights reserved
      </p>
    </div>
  </footer>
</template>

<script setup>
import SocialLinks from "./SocialLinks.vue";
</script>
