<script setup lang="ts">
import { useAuth } from '../composables/useAuth'

const { user, signOut } = useAuth()
</script>

<template>
  <div class="min-h-screen bg-gray-50">
    <!-- Header -->
    <header class="bg-white shadow-sm border-b border-gray-200">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex justify-between items-center h-16">
          <div class="flex items-center space-x-2">
            <div class="w-8 h-8 bg-gradient-to-br from-primary-500 to-secondary-500 rounded-lg flex items-center justify-center">
              <span class="text-white font-bold text-sm">IA</span>
            </div>
            <span class="text-xl font-bold text-gray-900">IA-Business</span>
          </div>
          
          <div class="flex items-center space-x-4">
            <img 
              :src="user?.user_metadata.avatar_url" 
              :alt="user?.user_metadata.full_name"
              class="w-8 h-8 rounded-full"
            />
            <span class="text-gray-700">{{ user?.user_metadata.full_name }}</span>
            <button 
              @click="signOut"
              class="text-gray-600 hover:text-red-600 transition-colors duration-200"
            >
              Salir
            </button>
          </div>
        </div>
      </div>
    </header>

    <!-- Main Content -->
    <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8">
      <div class="mb-8">
        <h1 class="text-3xl font-bold text-gray-900">
          ¡Bienvenido, {{ user?.user_metadata.full_name }}!
        </h1>
        <p class="text-gray-600 mt-2">
          Aquí está tu panel de control de IA-Business
        </p>
      </div>

      <!-- Dashboard Cards -->
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <div class="bg-white rounded-xl shadow-sm p-6 border border-gray-200">
          <div class="flex items-center justify-between mb-4">
            <h3 class="text-lg font-semibold text-gray-900">Proyectos Activos</h3>
            <div class="w-10 h-10 bg-primary-100 rounded-lg flex items-center justify-center">
              <svg class="w-5 h-5 text-primary-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10" />
              </svg>
            </div>
          </div>
          <div class="text-3xl font-bold text-gray-900 mb-2">12</div>
          <p class="text-sm text-gray-600">+2 desde el mes pasado</p>
        </div>

        <div class="bg-white rounded-xl shadow-sm p-6 border border-gray-200">
          <div class="flex items-center justify-between mb-4">
            <h3 class="text-lg font-semibold text-gray-900">Automatizaciones</h3>
            <div class="w-10 h-10 bg-green-100 rounded-lg flex items-center justify-center">
              <svg class="w-5 h-5 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
              </svg>
            </div>
          </div>
          <div class="text-3xl font-bold text-gray-900 mb-2">47</div>
          <p class="text-sm text-gray-600">Activas y funcionando</p>
        </div>

        <div class="bg-white rounded-xl shadow-sm p-6 border border-gray-200">
          <div class="flex items-center justify-between mb-4">
            <h3 class="text-lg font-semibold text-gray-900">Ahorro de Tiempo</h3>
            <div class="w-10 h-10 bg-orange-100 rounded-lg flex items-center justify-center">
              <svg class="w-5 h-5 text-orange-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
              </svg>
            </div>
          </div>
          <div class="text-3xl font-bold text-gray-900 mb-2">156h</div>
          <p class="text-sm text-gray-600">Este mes</p>
        </div>
      </div>

      <!-- Recent Activity -->
      <div class="mt-8 bg-white rounded-xl shadow-sm border border-gray-200">
        <div class="p-6 border-b border-gray-200">
          <h2 class="text-xl font-semibold text-gray-900">Actividad Reciente</h2>
        </div>
        <div class="p-6">
          <div class="space-y-4">
            <div class="flex items-center space-x-4">
              <div class="w-2 h-2 bg-green-500 rounded-full"></div>
              <div class="flex-1">
                <p class="text-sm text-gray-900">Automatización de emails configurada</p>
                <p class="text-xs text-gray-500">Hace 2 horas</p>
              </div>
            </div>
            <div class="flex items-center space-x-4">
              <div class="w-2 h-2 bg-blue-500 rounded-full"></div>
              <div class="flex-1">
                <p class="text-sm text-gray-900">Nuevo proyecto "Marketing IA" creado</p>
                <p class="text-xs text-gray-500">Hace 5 horas</p>
              </div>
            </div>
            <div class="flex items-center space-x-4">
              <div class="w-2 h-2 bg-purple-500 rounded-full"></div>
              <div class="flex-1">
                <p class="text-sm text-gray-900">Análisis predictivo completado</p>
                <p class="text-xs text-gray-500">Ayer</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>