<script setup>

const title = "dhiaaziz"
const links = [
  {
    "text": "cv and portfolios",
    "url": "https://drive.google.com/file/d/1cTfQwbYcGngRJrS5SeWk9eDUq0PJ_dOv/view?usp=sharing",
    "icon": `
    <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-book-download" width="18" height="18" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
   <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>
   <path d="M12 20h-6a2 2 0 0 1 -2 -2v-12a2 2 0 0 1 2 -2h12v5"></path>
   <path d="M13 16h-7a2 2 0 0 0 -2 2"></path>
   <path d="M15 19l3 3l3 -3"></path>
   <path d="M18 22v-9"></path>
</svg>`
  },
  {
    "text": "Github",
    "url": "https://github.com/dhiaaziz",
    "icon": `<svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-brand-github" width="18" height="18" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
   <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>
   <path d="M9 19c-4.3 1.4 -4.3 -2.5 -6 -3m12 5v-3.5c0 -1 .1 -1.4 -.5 -2c2.8 -.3 5.5 -1.4 5.5 -6a4.6 4.6 0 0 0 -1.3 -3.2a4.2 4.2 0 0 0 -.1 -3.2s-1.1 -.3 -3.5 1.3a12.3 12.3 0 0 0 -6.2 0c-2.4 -1.6 -3.5 -1.3 -3.5 -1.3a4.2 4.2 0 0 0 -.1 3.2a4.6 4.6 0 0 0 -1.3 3.2c0 4.6 2.7 5.7 5.5 6c-.6 .6 -.6 1.2 -.5 2v3.5"></path>
</svg>`
  },
]
</script>

<template>
  <div>
    <!-- <NuxtWelcome /> -->

    <div class="bg-gradient-to-r from-gray-900 to-teal-900 background-animate h-screen flex items-center justify-center flex-col">
      <div>
        <h1 class="tracking-widest mb-3 text-2xl">{{ title }}</h1>
      </div>
      <div>
        <a v-for="link in links" :href="link.url" target="_blank" class="btn btn-sm hover:text-teal-600 hover:border-teal-600 mx-2 bg-zinc-900"><span class="mr-1" v-if="link.icon" v-html="link.icon"></span>{{ link.text }}</a>
      </div>
    </div>
  </div>
</template>

<style scoped>
body {
  font-family: sans-serif;
}

.background-animate {
  background-size: 400%;

  -webkit-animation: AnimationName 30s ease infinite;
  -moz-animation: AnimationName 30s ease infinite;
  animation: AnimationName 30s ease infinite;
}

@keyframes AnimationName {

  0%,
  100% {
    background-position: 0% 50%;
  }

  50% {
    background-position: 100% 50%;
  }
}
</style>