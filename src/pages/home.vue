<template>
  <div class="bg-white pb-6 sm:pb-8 lg:pb-12">
  <div class="max-w-screen-2xl px-4 md:px-8 mx-auto">
   
    <section class="flex flex-col lg:flex-row justify-between gap-6 sm:gap-10 md:gap-16 mb-8 md:mb-16">
     
          <!-- image - start -->
      <div class="xl:w-5/12 h-48 lg:h-96 bg-gray-100 overflow-hidden shadow-lg rounded-lg">
       <img src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000" loading="lazy" alt="Photo by Fakurian Design" class="w-full h-full object-cover object-center" />
      </div>
      <!-- image - end -->
       <div class="xl:w-5/12 flex flex-col justify-center sm:text-center lg:text-left lg:py-12">
        <p class="text-indigo-500 md:text-lg xl:text-xl font-semibold mb-4 md:mb-6">Very proud to introduce</p>

        <h1 class="text-black-800 text-4xl sm:text-5xl md:text-6xl font-bold mb-8 md:mb-12"> way to build the web</h1>

        <div class="flex flex-col sm:flex-row sm:justify-center lg:justify-start gap-2.5">
          <a href="#" class="inline-block bg-indigo-500 hover:bg-indigo-600 active:bg-indigo-700 focus-visible:ring ring-indigo-300 text-white text-sm md:text-base font-semibold text-center rounded-lg outline-none transition duration-100 px-8 py-3">Start now</a>

          <a href="#" class="inline-block bg-indigo-500 hover:bg-indigo-600 active:bg-indigo-700 focus-visible:ring ring-indigo-300 text-white text-sm md:text-base font-semibold text-center rounded-lg outline-none transition duration-100 px-8 py-3">Start now</a>

          <a href="#" class="inline-block bg-gray-200 hover:bg-gray-300 focus-visible:ring ring-indigo-300 text-gray-500 active:text-gray-700 text-sm md:text-base font-semibold text-center rounded-lg outline-none transition duration-100 px-8 py-3">Take tour</a>
        </div>
      </div>


    </section>

    <section class="flex flex-col lg:flex-row justify-between items-center border-t gap-10 lg:gap-8 pt-8">
      <!-- stats - start -->
      <div class="grid grid-cols-2 md:flex md:divide-x gap-4 -mx-6 md:-mx-8">
        <div class="px-6 md:px-8">
          <span class="block text-indigo-500 text-lg md:text-xl font-bold text-center md:text-left">200</span>
          <span class="block text-gray-800 text-sm md:text-base font-semibold text-center md:text-left">People</span>
        </div>

        <div class="px-6 md:px-8">
          <span class="block text-indigo-500 text-lg md:text-xl font-bold text-center md:text-left">500+</span>
          <span class="block text-gray-800 text-sm md:text-base font-semibold text-center md:text-left">Projects</span>
        </div>

        <div class="px-6 md:px-8">
          <span class="block text-indigo-500 text-lg md:text-xl font-bold text-center md:text-left">250+</span>
          <span class="block text-gray-800 text-sm md:text-base font-semibold text-center md:text-left">Customers</span>
        </div>

        <div class="px-6 md:px-8">
          <span class="block text-indigo-500 text-lg md:text-xl font-bold text-center md:text-left">A couple</span>
          <span class="block text-gray-800 text-sm md:text-base font-semibold text-center md:text-left">Coffee breaks</span>
        </div>
      </div>
      <!-- stats - end -->

      <!-- social - start -->
      <div class="flex justify-center lg:justify-start items-center gap-4">
        <span class="text-gray-400 text-sm sm:text-base font-semibold tracking-widest uppercase">Social</span>
        <span class="w-12 h-px bg-gray-200"></span>

        <div class="flex gap-4">
          

           <a href="https://www.youtube.com/codeiiest" target="_blank" rel="noreferrer">
            <carbon-logo-facebook class="text-blue-500 hover:text-blue-600 transition duration-500 ease-in-out transform" aria-label="CodeIIEST YouTube Channel" />
          </a>
           <a href="https://www.youtube.com/codeiiest" target="_blank" rel="noreferrer">
            <carbon-logo-youtube class="text-red-500 hover:text-red-600 transition duration-500 ease-in-out transform" aria-label="CodeIIEST YouTube Channel" />
          </a>
           <a href="https://www.youtube.com/codeiiest" target="_blank" rel="noreferrer">
            <carbon-logo-linkedin  class="text-blue-500 hover:text-blue-600 transition duration-500 ease-in-out transform" aria-label="CodeIIEST YouTube Channel" />
          </a>
           <a href="https://www.youtube.com/codeiiest" target="_blank" rel="noreferrer">
            <carbon-logo-youtube class="text-red-500 hover:text-red-600 transition duration-500 ease-in-out transform" aria-label="CodeIIEST YouTube Channel" />
          </a>


         

        
        </div>
      </div>
      <!-- social - end -->
    </section>
  </div>
</div>

  

  <div class="text-center">
     <div class="mt-2">
      <h1
        class="
          dark:text-gray-100
          text-gray-900 text-3xl
          tracking-tight
          font-bold
        "
      >
        Business Insights
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
                <span> Read more <carbon-arrow-right aria-label="Chapter Details" class="inline" /></span>
              </router-link>
            </div>
          </div>
        </div>
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
