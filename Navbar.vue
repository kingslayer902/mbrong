<template>
    <nav class="bg-white shadow-md px-6 py-4 sticky top-0 z-50">
      <div class="flex justify-between items-center">
        <h1 class="text-2xl font-bold text-purple-600">MyMbrongSite</h1>
  
        <!-- Desktop Menu -->
        <div class="hidden md:flex space-x-6">
          <router-link to="/" class="text-gray-700 hover:text-purple-600 font-medium">Beranda</router-link>
          <router-link to="/about" class="text-gray-700 hover:text-purple-600 font-medium">Tentang</router-link>
          <router-link to="/contact" class="text-gray-700 hover:text-purple-600 font-medium">Kontak</router-link>
        </div>
  
        <!-- Hamburger Button (Mobile) -->
        <button class="md:hidden" @click="isOpen = !isOpen">
          <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16M4 18h16"/>
          </svg>
        </button>
      </div>
  
      <!-- Mobile Menu -->
      <div v-if="isOpen" class="md:hidden mt-4 space-y-2">
        <router-link @click="isOpen = false" to="/" class="block text-gray-700 hover:text-purple-600">Beranda</router-link>
        <router-link @click="isOpen = false" to="/about" class="block text-gray-700 hover:text-purple-600">Tentang</router-link>
        <router-link @click="isOpen = false" to="/contact" class="block text-gray-700 hover:text-purple-600">Kontak</router-link>
      </div>
    </nav>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  const isOpen = ref(false)
  </script>
  