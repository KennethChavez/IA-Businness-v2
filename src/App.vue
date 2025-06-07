<script setup lang="ts">
import { RouterView } from 'vue-router'
import { useAuth } from './composables/useAuth'

const { loading } = useAuth()
</script>

<template>
  <div id="app">
    <div v-if="loading" class="min-h-screen flex items-center justify-center bg-gray-50">
      <div class="animate-spin rounded-full h-12 w-12 border-b-2 border-primary-600"></div>
    </div>
    <RouterView v-else />
  </div>
</template>