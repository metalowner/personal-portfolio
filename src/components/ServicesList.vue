<script setup lang="ts">
import { BarChart3, Globe, ShieldCheck, PieChart } from '@lucide/vue'

const services = [
  {
    icon: BarChart3,
    title: "Маркетинг-стратегия и продажи под ключ",
    desc: "Полный цикл запуска продукта: выявление болей целевой аудитории, проектирование структуры лендингов, написание продающих текстов, создание скриптов продаж и сборка единой сквозной воронки."
  },
  {
    icon: Globe,
    title: "Разработка сайтов и приложений",
    desc: "Проектирование и техническая сборка чистых, современных сайтов и приложений с нуля. Закладываю правильную архитектуру, высокую скорость работы и полную готовность к запуску контекстной или таргетированной рекламы."
  },
  {
    icon: ShieldCheck,
    title: "Аудит сайтов и интерфейсов (UI/UX)",
    desc: "Глубокая ревизия вашего текущего сайта или лендинга. Проверяю удобство интерфейса для реальных людей, нахожу точки потери клиентов и даю четкие рекомендации, как повысить вероятность целевого действия."
  },
  {
    icon: PieChart,
    title: "Бизнес-планирование и автоматизация",
    desc: "Помогаю смоделировать бизнес-процессы, рассчитать юнит-экономику проекта и избавить команду от рутины. Проектирую умных Telegram-ботов для сотрудников и интегрирую таск-трекеры."
  }
]
</script>

<template>
  <section id="services" class="py-16 bg-slate-50 border-y border-slate-200 px-6 md:px-8">
    <div class="max-w-6xl mx-auto">
      <div class="text-center mb-12">
        <h2 class="text-3xl font-bold text-slate-900 tracking-tight">Чем я могу помочь вашему бизнесу</h2>
        <p class="text-sm font-semibold text-slate-400 uppercase tracking-wider mt-2">Решаю конкретные задачи без абстрактных обещаний</p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6 md:gap-8">
        <div 
          v-for="(service, idx) in services" 
          :key="idx"
          class="bg-white p-6 rounded-2xl border border-slate-200/60 shadow-sm flex flex-col sm:flex-row gap-5 transition-all hover:shadow-md"
        >
          <div class="p-3 bg-indigo-50 text-indigo-600 rounded-xl h-fit w-fit shrink-0">
            <component :is="service.icon" class="w-6 h-6" />
          </div>
          <div class="flex flex-col gap-2">
            <h3 class="font-bold text-slate-800 text-base md:text-lg leading-snug">{{ service.title }}</h3>
            <p class="text-xs md:text-sm text-slate-500 leading-relaxed font-medium">{{ service.desc }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
