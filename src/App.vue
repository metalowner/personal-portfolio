<script setup lang="ts">
import HeroSection from './components/HeroSection.vue'
import ServicesList from './components/ServicesList.vue'
import FrameworkApproach from './components/FrameworkApproach.vue'
import CaseStudies from './components/CaseStudies.vue'
import { Sparkles } from '@lucide/vue'
</script>

<template>
  <div class="min-h-screen bg-brand-bg text-slate-800 flex flex-col">
    <!-- Clean Minimalist Header -->
    <header class="border-b border-brand-border px-6 md:px-8 py-4 bg-brand-card flex justify-between items-center shadow-sm sticky top-0 z-50">
      <div class="flex items-center gap-2.5">
        <div class="bg-indigo-600 p-2 rounded-xl text-white shadow-sm">
          <Sparkles class="w-4 h-4" />
        </div>
        <span class="font-bold text-slate-900 tracking-tight text-base md:text-lg">Павел Юдкевич</span>
      </div>
      <a 
        href="https://t.me" 
        target="_blank"
        class="text-xs font-bold bg-indigo-50 hover:bg-indigo-100 text-indigo-700 border border-indigo-100 px-4 py-2 rounded-xl transition-all cursor-pointer"
      >
        Связаться
      </a>
    </header>

    <!-- Content Sections -->
    <main class="flex-1 flex flex-col">
      <HeroSection />
      <ServicesList />
      <FrameworkApproach />
      <CaseStudies />
    </main>

    <!-- Footer -->
    <footer class="border-t border-brand-border bg-brand-card py-8 px-6 text-center text-xs font-medium text-slate-400">
      © 2026 Павел Юдкевич. Спроектировано и написано вручную на Vue 3 & Tailwind CSS v4.
    </footer>
  </div>
</template>
