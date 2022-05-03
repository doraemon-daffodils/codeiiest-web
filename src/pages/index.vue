<template>
  <div class="text-center">
    <h1
      class="
        dark:text-gray-100
        text-gray-900 text-4xl
        tracking-tight
        font-extrabold
        sm:text-5xl
        md:text-6xl
        cursor-default
      "
    >
      <span class="block xl:inline">Code</span>
      <!-- space -->
      <span class="block text-red-600 xl:inline">IIEST</span>
    </h1>
    <p
      class="
        mt-3
        max-w-md
        mx-auto
        text-base text-gray-500
        dark:text-gray-400
        sm:text-lg
        md:mt-5
        md:text-xl
        md:max-w-3xl
        cursor-default
      "
    >
      The Coding Club of IIEST, Shibpur.
      <br /><br />
      CodeIIEST is one of the newest clubs of the <span class="font-bold">Indian Institute of Engineering Science and Technology, Shibpur</span>. Since its inception in November of 2014, the club has been actively involved in the development of comprehensive computer science abilities among students. The group is made up of a variety of interests and serves as a fantastic hub for a variety of instructive and interactive programs. The students stay up to date on new technology, which helps them improve their skills and foster creativity and innovation.
    </p>
    <div class="mt-15">
      <h1
        class="
          dark:text-gray-100
          text-gray-900 text-3xl
          tracking-tight
          font-bold
        "
      >
        Chapters
      </h1>
      <div class="flex flex-wrap justify-center mt-5">
        <div
          v-for="(chapter, index) in chapters"
          :key="index"
          class="
            w-full
            max-w-sm
            px-4
            py-3
            mx-5
            my-3
            bg-white
            rounded-md
            shadow-md
            transition duration-300
            hover:shadow-lg hover:shadow-red-500
            dark:hover:shadow-red-200
            dark:bg-dark-800
          "
        >
          <div>
            <h1
              class="mt-2 text-lg font-semibold text-gray-800 dark:text-white"
            >
              {{ chapter.name }}
            </h1>
            <p
              class="
                mt-2
                text-sm text-gray-600
                dark:text-gray-300
                cursor-default
              "
            >
              {{ chapter.descp }}
            </p>
          </div>

          <div>
            <div
              class="flex justify-center mt-2 text-gray-700 dark:text-gray-200"
            >
              <router-link
                :to="chapter.route"
                class="
                  mx-2
                  text-red-600
                  cursor-pointer
                  dark:text-red-400
                  hover:underline
                "
              >
                <span>Chapter Details<carbon-arrow-right aria-label="Chapter Details" class="inline" /></span>
              </router-link>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  
<div class="fixed bottom-0 left-0 p-4 w-full z-50">
  <div class="max-w-screen-md ring-3 dark:ring-gray-900 ring-white text-white mx-auto flex flex-col md:flex-row space-y-4 md:space-y-0 relative justify-between items-center rounded-3xl bg-gray-800 p-4">
    <div class="flex items-center space-x-4">
      <div class="p-3 rounded-2xl bg-white/5 text-white">
</div> 
    <span> Utilizamos <b>cookies</b> para mejorar la experiencia enel sitio web.
      <a href="#" class="order-last sm:order-none w-full sm:w-auto inline-block bg-indigo-600 hover:bg-indigo-700 active:bg-indigo-800 focus-visible:ring ring-indigo-300 text-white text-xs md:text-sm font-semibold text-center whitespace-nowrap rounded-lg outline-none transition duration-100 px-4 py-2">Learn more</a>
     </span>
     </div>
 </div>
 </div>
</template>

<script setup lang="ts">
import { chapters } from '~/logic'
</script>

<route lang="yaml">
meta:
  layout: default
</route>
