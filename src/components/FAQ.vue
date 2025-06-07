<template>
  <section id="faq" class="py-20 bg-gray-50">
    <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-3xl sm:text-4xl font-bold text-gray-900 mb-4">
          Preguntas Frecuentes
        </h2>
        <p class="text-xl text-gray-600">
          Resolvemos las dudas más comunes sobre nuestro CRM de WhatsApp con IA
        </p>
      </div>

      <div class="space-y-6">
        <div 
          v-for="(faq, index) in faqs" 
          :key="index"
          class="bg-white rounded-xl shadow-sm border border-gray-200 overflow-hidden"
        >
          <button 
            @click="toggleFAQ(index)"
            class="w-full px-6 py-4 text-left flex justify-between items-center hover:bg-gray-50 transition-colors duration-200"
          >
            <h3 class="text-lg font-semibold text-gray-900">{{ faq.question }}</h3>
            <svg 
              :class="{ 'rotate-180': faq.isOpen }"
              class="w-5 h-5 text-gray-500 transform transition-transform duration-200"
              fill="none" 
              stroke="currentColor" 
              viewBox="0 0 24 24"
            >
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
            </svg>
          </button>
          <div 
            v-show="faq.isOpen"
            class="px-6 pb-4 text-gray-600 leading-relaxed"
          >
            {{ faq.answer }}
          </div>
        </div>
      </div>

      <!-- Contact CTA -->
      <div class="mt-12 text-center">
        <p class="text-gray-600 mb-6">¿No encuentras la respuesta que buscas?</p>
        <a 
          href="https://api.whatsapp.com/send?phone=+50489424660&text=Hola,%20quiero%20m%C3%A1s%20informaci%C3%B3n%20sobre%20Honduras%20IA%202025"
          target="_blank"
          class="inline-flex items-center space-x-2 bg-gradient-to-r from-green-500 to-blue-500 text-white px-8 py-3 rounded-xl font-semibold hover:shadow-lg transform hover:scale-105 transition-all duration-200"
        >
          <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
            <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893A11.821 11.821 0 0020.885 3.488"/>
          </svg>
          <span>Contáctanos por WhatsApp</span>
        </a>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const faqs = ref([
  {
    question: "¿Qué es WhatsApp Business API y cómo funciona?",
    answer: "WhatsApp Business API es la versión oficial de WhatsApp para empresas que permite enviar mensajes automatizados, crear chatbots y gestionar conversaciones a gran escala. Nuestro sistema se conecta directamente con esta API para automatizar todas tus comunicaciones.",
    isOpen: false
  },
  {
    question: "¿Necesito conocimientos técnicos para usar IA-Business?",
    answer: "No, nuestro sistema está diseñado para ser intuitivo y fácil de usar. Incluye plantillas predefinidas, flujos visuales y una interfaz amigable. Además, ofrecemos capacitación completa y soporte técnico 24/7.",
    isOpen: false
  },
  {
    question: "¿Puedo integrar mi CRM actual con IA-Business?",
    answer: "Sí, ofrecemos integraciones con los principales CRM del mercado como Salesforce, HubSpot, Pipedrive y muchos más. También tenemos API abierta para integraciones personalizadas.",
    isOpen: false
  },
  {
    question: "¿Cómo funciona el chatbot con inteligencia artificial?",
    answer: "Nuestro chatbot utiliza procesamiento de lenguaje natural (NLP) y machine learning para entender las consultas de los clientes y responder de manera inteligente. Aprende continuamente de las conversaciones para mejorar sus respuestas.",
    isOpen: false
  },
  {
    question: "¿Qué tipos de flujos automatizados puedo crear?",
    answer: "Puedes crear flujos para ventas, soporte al cliente, reservas de citas, recordatorios de pago, encuestas de satisfacción, seguimiento post-venta y mucho más. Todo con un editor visual fácil de usar.",
    isOpen: false
  },
  {
    question: "¿Es seguro usar WhatsApp para mi negocio?",
    answer: "Absolutamente. WhatsApp Business API cumple con los más altos estándares de seguridad y privacidad. Todos los mensajes están encriptados de extremo a extremo y cumplimos con GDPR y otras regulaciones de protección de datos.",
    isOpen: false
  },
  {
    question: "¿Cuánto cuesta implementar IA-Business?",
    answer: "Ofrecemos planes flexibles desde $29/mes para pequeñas empresas hasta soluciones empresariales personalizadas. El costo incluye la plataforma, soporte técnico y actualizaciones. Contáctanos para una cotización personalizada.",
    isOpen: false
  },
  {
    question: "¿Ofrecen soporte en español?",
    answer: "Sí, todo nuestro equipo de soporte habla español y está disponible 24/7 para ayudarte. Ofrecemos soporte por WhatsApp, email, chat en vivo y videollamadas.",
    isOpen: false
  }
])

const toggleFAQ = (index: number) => {
  faqs.value[index].isOpen = !faqs.value[index].isOpen
}
</script>