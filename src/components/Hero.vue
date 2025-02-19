<template>
    <section class="min-h-screen flex flex-col justify-center relative px-4 sm:px-6 lg:px-8 pt-16">
        <div class="text-center">
          <h1  class="text-5xl sm:text-7xl font-bold mb-4 tracking-tight">
              <span class="bg-clip-text text-transparent bg-gradient-to-r from-purple-400 to-pink-500">
                Richard Browne
              </span>
          </h1>

          <p class="text-2xl sm:text-3xl text-gray-400 mb-4">Software Engineer</p>

          <!-- Icons -->
          <div class="flex justify-center gap-6">
            <a href="https://github.com/DroneBreaker" class="text-gray-400 hover:text-purple-400 transition-colors">
              <Github class="w-6 h-6" />
            </a>
            
            <a href="https://linkedin.com/in/therichardbrowne" class="text-gray-400 hover:text-purple-400 transition-colors">
              <Linkedin class="w-6 h-6" />
            </a>

            <a href="mailto:brownierz01@gmail.com" class="text-gray-400 hover:text-purple-400 transition-colors">
              <Mail class="w-6 h-6" />
            </a>

            <a href="/src/assets/richardbrowne.pdf" download="/src/assets/richardbrowne.pdf" class="text-gray-400 hover:text-purple-400 transition-colors">
              <File class="w-6 h-6" />
            </a>
          </div>
        </div>

        <ArrowDown class="tracking-tight self-center mt-[10rem] w-8 h-8 bg-clip-content content-transparent bg-gradient-to-r from-purple-400 to-pink-500" />
    </section>
</template>

<script setup>
import { Github, Linkedin, Mail, File, ArrowDown } from 'lucide-vue-next'
</script>

<style lang="scss" scoped>

</style>