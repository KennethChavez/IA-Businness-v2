<template>
  <footer class="bg-gray-900 text-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
      <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
        <!-- Company Info -->
        <div class="col-span-1 md:col-span-2">
          <div class="flex items-center space-x-2 mb-6">
            <div class="w-8 h-8 bg-gradient-to-br from-green-500 to-blue-500 rounded-lg flex items-center justify-center">
              <span class="text-white font-bold text-sm">IA</span>
            </div>
            <span class="text-xl font-bold">IA-Business</span>
          </div>
          <p class="text-gray-400 mb-6 max-w-md">
            Automatiza tu WhatsApp Business con IA. La solución más avanzada para 
            chatbots, CRM y flujos automatizados en WhatsApp.
          </p>
          
          <!-- Contact Info -->
          <div class="space-y-3 mb-6">
            <div class="flex items-center space-x-3">
              <svg class="w-5 h-5 text-green-500" fill="currentColor" viewBox="0 0 24 24">
                <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893A11.821 11.821 0 0020.885 3.488"/>
              </svg>
              <a 
                href="https://api.whatsapp.com/send?phone=+50489424660&text=Hola,%20quiero%20m%C3%A1s%20informaci%C3%B3n%20sobre%20Honduras%20IA%202025"
                target="_blank"
                class="text-gray-400 hover:text-green-400 transition-colors duration-200"
              >
                WhatsApp: +504 8942-4660
              </a>
            </div>
            
            <div class="flex items-center space-x-3">
              <svg class="w-5 h-5 text-blue-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
              </svg>
              <span class="text-gray-400">+504 8942-4660</span>
            </div>
          </div>
          
          <div class="flex space-x-4">
            <a 
              href="https://api.whatsapp.com/send?phone=+50489424660&text=Hola,%20quiero%20m%C3%A1s%20informaci%C3%B3n%20sobre%20Honduras%20IA%202025"
              target="_blank"
              class="text-gray-400 hover:text-green-400 transition-colors duration-200"
            >
              <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893A11.821 11.821 0 0020.885 3.488"/>
              </svg>
            </a>
            <a href="#" class="text-gray-400 hover:text-white transition-colors duration-200">
              <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                <path d="M22.46 6c-.77.35-1.6.58-2.46.69.88-.53 1.56-1.37 1.88-2.38-.83.5-1.75.85-2.72 1.05C18.37 4.5 17.26 4 16 4c-2.35 0-4.27 1.92-4.27 4.29 0 .34.04.67.11.98C8.28 9.09 5.11 7.38 3 4.79c-.37.63-.58 1.37-.58 2.15 0 1.49.75 2.81 1.91 3.56-.71 0-1.37-.2-1.95-.5v.03c0 2.08 1.48 3.82 3.44 4.21a4.22 4.22 0 0 1-1.93.07 4.28 4.28 0 0 0 4 2.98 8.521 8.521 0 0 1-5.33 1.84c-.34 0-.68-.02-1.02-.06C3.44 20.29 5.7 21 8.12 21 16 21 20.33 14.46 20.33 8.79c0-.19 0-.37-.01-.56.84-.6 1.56-1.36 2.14-2.23z"/>
              </svg>
            </a>
            <a href="#" class="text-gray-400 hover:text-white transition-colors duration-200">
              <!-- Botón que redirige a Dashboard -->
              <router-link to="/dashboard">
                <button class="bg-primary-600 hover:bg-primary-700 text-white font-bold py-2 px-4 rounded transition-colors duration-200">
                  Ir al Dashboard
                </button>
              </router-link>
            </a>
          </div>
        </div>

        <!-- Product -->
        <div>
          <h3 class="text-lg font-semibold mb-6">Producto</h3>
          <ul class="space-y-4">
            <li><a href="#features" class="text-gray-400 hover:text-white transition-colors duration-200">Características</a></li>
            <li><a href="#pricing" class="text-gray-400 hover:text-white transition-colors duration-200">Precios</a></li>
            <li><a href="#faq" class="text-gray-400 hover:text-white transition-colors duration-200">FAQ</a></li>
            <li><a href="https://developers.facebook.com/docs/whatsapp/cloud-api" target="_blank" class="text-gray-400 hover:text-white transition-colors duration-200">WhatsApp API</a></li>
          </ul>
        </div>

        <!-- Support -->
        <div>
          <h3 class="text-lg font-semibold mb-6">Soporte</h3>
          <ul class="space-y-4">
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-200">Centro de ayuda</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-200">Documentación</a></li>
            <li>
              <a 
                href="https://api.whatsapp.com/send?phone=+50489424660&text=Hola,%20quiero%20m%C3%A1s%20informaci%C3%B3n%20sobre%20Honduras%20IA%202025"
                target="_blank"
                class="text-gray-400 hover:text-green-400 transition-colors duration-200"
              >
                Contacto WhatsApp
              </a>
            </li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-200">Estado del servicio</a></li>
          </ul>
        </div>
      </div>

      <div class="border-t border-gray-800 mt-12 pt-8 flex flex-col md:flex-row justify-between items-center">
        <p class="text-gray-400 text-sm">
          © 2025 IA-Business. Todos los derechos reservados.
        </p>
        <div class="flex space-x-6 mt-4 md:mt-0">
          <a href="#" class="text-gray-400 hover:text-white text-sm transition-colors duration-200">
            Política de privacidad
          </a>
          <a href="#" class="text-gray-400 hover:text-white text-sm transition-colors duration-200">
            Términos de servicio
          </a>
        </div>
      </div>
    </div>
  </footer>
</template>