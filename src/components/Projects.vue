<template>
    <div class="bg-black">
        <hr class="bg-white">
        <h1 class="text-4xl text-white font-bold text-center pt-6 mb-12">
            {{ projectsIntro }}
        </h1>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 mx-12 cursor-pointer gap-8">
            <div v-for="project in projects" :key="project.title" class="rounded-xl transition-all bg-gray-900 border-gray-700 mb-4">
                <img class="h-[17rem] rounded-t-xl w-full" :src="project.image" :alt="project.title">

                <div class="p-6">
                    <h3 class="mb-2">{{ project.title }}</h3>

                    <!-- Description -->
                    <p class="mb-4">{{ project.description }}</p>
                    
                    <!-- Tags Div -->
                    <div class="flex flex-wrap gap-2 mb-4">
                        <span 
                            v-for="tag in project.tags" 
                            :key="tag"
                            class="px-3 py-1 bg-gray-800 text-purple-400 rounded-full text-sm"
                        >
                        {{ tag }}
                        </span>
                    </div>

                    <div class="flex justify-between">
                        <a :href="project.github" class="flex items-center text-gray-400 hover:text-purple-400">
                            <Github class="w-5 h-5 mr-2" />
                            Code
                        </a>
                </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';
import  { Github } from 'lucide-vue-next'

// Define props to accept the projects intro from the parent component
const props = defineProps({
    projectsIntro: {
        type: String,
        required: true,
        default: 'Featured Projects'
    }
})

const projects = ref([
    { 
        title: 'Travel Booking App', 
        description: 'A travel booking application that was built with Flutter and Firebase.', 
        image: '/src/assets/travel.jpg', 
        tags: ['Flutter', 'Firebase'],
        github: 'https://github.com/DroneBreaker/Flutter-Travel-Booking-App' 
    },

    { 
        title: 'Invoicing App', 
        description: 'An invoicing application that was built with Flutter and Golang.', 
        image: '/src/assets/invoicing.jpg', 
        tags: ['Flutter', 'Golang'], 
        github: 'https://github.com/DroneBreaker/Flutter-Invoice-App' 
    },

    { 
        title: 'Admin Dashboard', 
        description: 'An ongoing admin dashboard with Vue and Golang.', 
        image: '/src/assets/admin.avif', 
        tags: ['Vue', 'Golang'], 
        github: 'https://github.com/DroneBreaker/Admin-Dashboard-App' 
    },
])
</script>

<style lang="scss" scoped>

</style>