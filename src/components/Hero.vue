<template>
    <section class="min-h-screen flex flex-col justify-center relative px-4 sm:px-6 lg:px-8">
        <div class="text-center">
            <h1  class="text-6xl sm:text-5xl font-bold mb-6 tracking-tight">
                <span class="bg-clip-text text-transparent bg-gradient-to-r from-purple-400 to-pink-500">
                  Richard Browne
                </span>
            </h1>

            <p class="text-2xl sm:text-2xl text-gray-400 mb-8">Software Engineer</p>

            <!-- Icons -->
            <div class="flex justify-center gap-6 mb-12">
            <a href="https://github.com/DroneBreaker" class="text-gray-400 hover:text-purple-400 transition-colors">
              <Github class="w-6 h-6" />
            </a>
            <a href="https://linkedin.com/in/therichardbrowne" class="text-gray-400 hover:text-purple-400 transition-colors">
              <Linkedin class="w-6 h-6" />
            </a>
            <a href="mailto:brownierz01@gmail.com" class="text-gray-400 hover:text-purple-400 transition-colors">
              <Mail class="w-6 h-6" />
            </a>
          </div>
        </div>
    </section>
</template>

<script setup>
import { Github, Linkedin, Mail, ExternalLink, Send } from 'lucide-vue-next'
</script>

<style lang="scss" scoped>

</style>