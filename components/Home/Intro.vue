<template>
  <div class="space-y-6">
    <Img src="/images/avatar.png" alt="Gavin Earley"
      class="ring-2 border ring-gray-200 border-gray-300 dark:ring-white/10 dark:border-gray-800 hover:ring-4 transition-all duration-300 bg-gray-200 dark:bg-gray-900 rounded-full h-12 w-12 sm:h-16 sm:w-16"
      sizes="48px sm:64px" placeholder format="webp" />
    <h1 class="text-xl font-bold tracking-tight text-gray-800 dark:text-gray-100">
      Hello!
    </h1>
    <p class="text-gray-900 dark:text-gray-400">
      Hello, my name is Gavin Earley
    </p>

    <h2 class="text-xl font-bold tracking-tight text-gray-800 dark:text-gray-100">
      Software should always be for helping people and never inhibit a user from what they are trying to accomplish.
      As a software engineer I strive to build great software that gets out of the way to let the user
      do what they need to do and be on their way. 
    </h2>

  </div>
</template>

<script setup>
useSeoMeta({
  title: "Gavin Earley",
  description:
    "I'm Gavin, software engineer, father, photographer and licensed drone pilot",
});
</script>
