<script setup lang="ts">
import { ArrowRight } from '@lucide/vue'
</script>

<template>
  <section class="py-20 px-6 md:px-8 max-w-5xl mx-auto text-center flex flex-col items-center gap-6">
    <div class="inline-flex items-center gap-2 px-3 py-1.5 bg-indigo-50 text-indigo-700 text-xs font-bold rounded-xl border border-indigo-100 uppercase tracking-wider">
      🤝 Совместная разработка и консалтинг
    </div>
    
    <h1 class="text-4xl md:text-5xl lg:text-6xl font-extrabold tracking-tight text-slate-900 leading-tight max-w-4xl">
      Разрабатываю сайты, создаю системы продаж и запускаю маркетинг.
    </h1>
    
    <p class="text-lg md:text-xl text-slate-500 max-w-2xl font-medium leading-relaxed">
      Без сложного ИТ-жаргона. Рука об руку с вами. Помогаю превратить идеи вашего бизнеса в прибыльные цифровые продукты и автоматизировать хаос.
    </p>

    <div class="flex flex-col sm:flex-row gap-4 mt-4 w-full sm:w-auto">
      <a 
        href="https://t.me" 
        target="_blank"
        class="bg-indigo-600 hover:bg-indigo-700 text-white font-semibold px-6 py-3.5 rounded-xl shadow-md shadow-indigo-600/10 flex items-center justify-center gap-2 transition-all active:scale-[0.99]"
      >
        Обсудить ваш проект
        <ArrowRight class="w-4 h-4" />
      </a>
      <a 
        href="#services" 
        class="bg-white hover:bg-slate-50 text-slate-700 border border-slate-200 font-semibold px-6 py-3.5 rounded-xl flex items-center justify-center gap-2 transition-all"
      >
        Посмотреть услуги
      </a>
    </div>
  </section>
</template>
