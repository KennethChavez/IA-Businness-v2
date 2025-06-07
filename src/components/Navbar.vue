<script setup lang="ts">
import { useAuth } from '../composables/useAuth'

const { user, signOut } = useAuth()
</script>

<template>
  <nav class="fixed w-full top-0 z-50 bg-white/80 backdrop-blur-md border-b border-gray-100">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center h-16">
        <!-- Logo -->
        <div class="flex items-center">
          <div class="flex items-center space-x-2">
            <div class="w-8 h-8 bg-gradient-to-br from-primary-500 to-secondary-500 rounded-lg flex items-center justify-center">
              <span class="text-white font-bold text-sm">IA</span>
            </div>
            <span class="text-xl font-bold text-gray-900">IA-Business</span>
          </div>
        </div>

        <!-- Navigation Links -->
        <div class="hidden md:flex items-center space-x-8">
          <a href="#features" class="text-gray-600 hover:text-primary-600 transition-colors duration-200">
            Características
          </a>
          <a href="#pricing" class="text-gray-600 hover:text-primary-600 transition-colors duration-200">
            Precios
          </a>
          <a href="#about" class="text-gray-600 hover:text-primary-600 transition-colors duration-200">
            Acerca de
          </a>
        </div>

        <!-- Auth Buttons -->
        <div class="flex items-center space-x-4">
          <template v-if="!user">
            <button class="text-gray-600 hover:text-primary-600 transition-colors duration-200">
              Iniciar Sesión
            </button>
            <button class="bg-gradient-to-r from-primary-500 to-secondary-500 text-white px-6 py-2 rounded-lg hover:shadow-lg transform hover:scale-105 transition-all duration-200">
              Registrarse
            </button>
          </template>
          <template v-else>
            <div class="flex items-center space-x-3">
              <img 
                :src="user.user_metadata.avatar_url" 
                :alt="user.user_metadata.full_name"
                class="w-8 h-8 rounded-full"
              />
              <span class="text-gray-700">{{ user.user_metadata.full_name }}</span>
              <button 
                @click="signOut"
                class="text-gray-600 hover:text-red-600 transition-colors duration-200"
              >
                Salir
              </button>
            </div>
          </template>
        </div>
      </div>
    </div>
  </nav>
</template>