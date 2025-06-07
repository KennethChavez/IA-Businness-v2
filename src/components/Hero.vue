<script setup lang="ts">
import { useAuth } from '../composables/useAuth'

const { signInWithGoogle } = useAuth()
</script>

<template>
  <section class="relative pt-24 pb-16 overflow-hidden">
    <!-- Background Pattern -->
    <div class="absolute inset-0 bg-gradient-to-br from-green-50 via-white to-blue-50">
      <div class="absolute inset-0 opacity-30">
        <div class="absolute top-0 left-0 w-72 h-72 bg-gradient-to-br from-green-200 to-blue-200 rounded-full mix-blend-multiply filter blur-xl animate-float"></div>
        <div class="absolute top-0 right-0 w-72 h-72 bg-gradient-to-br from-blue-200 to-green-200 rounded-full mix-blend-multiply filter blur-xl animate-float" style="animation-delay: 2s"></div>
        <div class="absolute bottom-0 left-1/2 w-72 h-72 bg-gradient-to-br from-green-200 to-blue-200 rounded-full mix-blend-multiply filter blur-xl animate-float" style="animation-delay: 4s"></div>
      </div>
    </div>

    <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
        <!-- Content -->
        <div class="text-center lg:text-left animate-slide-up">
          <div class="flex items-center justify-center lg:justify-start space-x-2 mb-6">
            <svg class="w-8 h-8 text-green-500" fill="currentColor" viewBox="0 0 24 24">
              <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893A11.821 11.821 0 0020.885 3.488"/>
            </svg>
            <span class="text-lg font-semibold text-gray-700">WhatsApp Business API</span>
          </div>
          
          <h1 class="text-4xl sm:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight">
            Automatiza tu 
            <span class="bg-gradient-to-r from-green-600 to-blue-600 bg-clip-text text-transparent">
              WhatsApp Business
            </span>
            con IA
          </h1>
          
          <p class="mt-6 text-xl text-gray-600 leading-relaxed">
            Conecta, automatiza y convierte más clientes con nuestro CRM inteligente. 
            Chatbots con IA, flujos automatizados, reservas y recordatorios en WhatsApp.
          </p>

          <div class="mt-10 flex flex-col sm:flex-row gap-4 justify-center lg:justify-start">
            <button 
              @click="signInWithGoogle"
              class="bg-gradient-to-r from-green-500 to-blue-500 text-white px-8 py-4 rounded-xl font-semibold hover:shadow-2xl transform hover:scale-105 transition-all duration-300 flex items-center justify-center space-x-2"
            >
              <svg class="w-5 h-5" viewBox="0 0 24 24">
                <path fill="currentColor" d="M22.56 12.25c0-.78-.07-1.53-.2-2.25H12v4.26h5.92c-.26 1.37-1.04 2.53-2.21 3.31v2.77h3.57c2.08-1.92 3.28-4.74 3.28-8.09z"/>
                <path fill="currentColor" d="M12 23c2.97 0 5.46-.98 7.28-2.66l-3.57-2.77c-.98.66-2.23 1.06-3.71 1.06-2.86 0-5.29-1.93-6.16-4.53H2.18v2.84C3.99 20.53 7.7 23 12 23z"/>
                <path fill="currentColor" d="M5.84 14.09c-.22-.66-.35-1.36-.35-2.09s.13-1.43.35-2.09V7.07H2.18C1.43 8.55 1 10.22 1 12s.43 3.45 1.18 4.93l2.85-2.22.81-.62z"/>
                <path fill="currentColor" d="M12 5.38c1.62 0 3.06.56 4.21 1.64l3.15-3.15C17.45 2.09 14.97 1 12 1 7.7 1 3.99 3.47 2.18 7.07l3.66 2.84c.87-2.6 3.3-4.53 6.16-4.53z"/>
              </svg>
              <span>Comenzar Gratis</span>
            </button>
            
            <a 
              href="https://api.whatsapp.com/send?phone=+50489424660&text=Hola,%20quiero%20m%C3%A1s%20informaci%C3%B3n%20sobre%20Honduras%20IA%202025"
              target="_blank"
              class="border-2 border-green-500 text-green-600 px-8 py-4 rounded-xl font-semibold hover:bg-green-50 transition-all duration-300 flex items-center justify-center space-x-2"
            >
              <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893A11.821 11.821 0 0020.885 3.488"/>
              </svg>
              <span>Hablar por WhatsApp</span>
            </a>
          </div>

          <!-- Stats -->
          <div class="mt-16 grid grid-cols-3 gap-6 lg:gap-8">
            <div class="text-center">
              <div class="text-2xl lg:text-3xl font-bold text-gray-900">4+</div>
              <div class="text-sm text-gray-600">Empresas conectadas</div>
              <div class="text-sm text-gray-600">En el primer trimestre</div>
            </div>
            <div class="text-center">
              <div class="text-2xl lg:text-3xl font-bold text-gray-900">98%</div>
              <div class="text-sm text-gray-600">Tasa de respuesta</div>
            </div>
            <div class="text-center">
              <div class="text-2xl lg:text-3xl font-bold text-gray-900">24/7</div>
              <div class="text-sm text-gray-600">Chatbot activo</div>
            </div>
          </div>
        </div>

        <!-- WhatsApp Interface Mockup -->
        <div class="relative animate-fade-in" style="animation-delay: 0.3s">
          <div class="relative">
            <img 
              src="https://files.selar.co/product-images/2022/products/nifemiojo/customized-whatsapp-bot-selar.co-621c48fa5bb79.png" 
              alt="WhatsApp Bot Interface"
              class="w-full h-auto rounded-2xl shadow-2xl"
            />
            <div class="absolute inset-0 bg-gradient-to-t from-green-500/20 to-transparent rounded-2xl"></div>
          </div>
          
          <!-- Floating Cards -->
          <div class="absolute -top-6 -right-6 bg-white/90 backdrop-blur-md p-4 rounded-xl shadow-lg animate-float">
            <div class="flex items-center space-x-3">
              <div class="w-3 h-3 bg-green-500 rounded-full animate-pulse"></div>
              <span class="text-sm font-medium text-gray-700">Bot Activo</span>
            </div>
          </div>
          
          <div class="absolute -bottom-6 -left-6 bg-white/90 backdrop-blur-md p-4 rounded-xl shadow-lg animate-float" style="animation-delay: 3s">
            <div class="text-sm text-gray-600">Conversiones</div>
            <div class="text-xl font-bold text-green-600">+200%</div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>