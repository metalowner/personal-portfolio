<script setup lang="ts">
import { ExternalLink } from 'lucide-vue-next'

const cases = [
  {
    tag: "Бизнес-инжиниринг и Франчайзинг",
    title: "Разработка комплексной системы продаж под ключ",
    desc: "Проектирование сквозной автоматизации процессов, маркетинговой воронки и структуры скриптов продаж для масштабирования коммерческой франшизы.",
    link: null
  },
  {
    tag: "AI & Full-Stack Автоматизация",
    title: "AI-Driven Jira Ассистент декомпозиции требований",
    desc: "Разработка веб-сервиса, преобразующего сырые концепты в готовый бэклог User Stories с критериями приемки с использованием ИИ. Исключает рутину планирования.",
    link: "https://github.com"
  },
  {
    tag: "Аналитика процессов и Метрики",
    title: "Интерактивный дашборд Agile-эффективности",
    desc: "Сборка панели мониторинга здоровья команд с симулятором процессов. Показывает предсказуемость спринтов, Cycle Time и графики Burndown/Velocity.",
    link: "https://github.com"
  },
  {
    tag: "Операционная Оптимизация",
    title: "Асинхронный бот сбора Daily-статусов команд",
    desc: "Создание Telegram-бота на Python, собирающего апдейты у удаленных сотрудников. Избавляет команду от лишних созвонов, генерируя красивые Markdown-отчеты.",
    link: "https://github.com"
  }
]
</script>

<template>
  <section class="py-16 bg-slate-50 border-t border-slate-200 px-6 md:px-8">
    <div class="max-w-5xl mx-auto">
      <div class="text-center mb-12">
        <h2 class="text-3xl font-bold text-slate-900 tracking-tight">Реализованные кейсы и проекты</h2>
        <p class="text-sm font-semibold text-slate-400 uppercase tracking-wider mt-2">Примеры систем, которые я проектирую и запускаю</p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div 
          v-for="(item, idx) in cases" 
          :key="idx"
          class="bg-white p-6 rounded-2xl border border-slate-200 shadow-sm flex flex-col justify-between gap-4"
        >
          <div class="flex flex-col gap-2">
            <span class="text-[10px] font-extrabold text-indigo-600 bg-indigo-50 px-2.5 py-0.5 rounded-md border border-indigo-100/50 uppercase tracking-wider w-fit">
              {{ item.tag }}
            </span>
            <h3 class="font-bold text-slate-800 text-base md:text-lg leading-snug mt-1">{{ item.title }}</h3>
            <p class="text-xs md:text-sm text-slate-500 font-medium leading-relaxed">{{ item.desc }}</p>
          </div>
          
          <div class="pt-2 border-t border-slate-100 mt-2">
            <a 
              v-if="item.link" 
              :href="item.link" 
              target="_blank"
              class="inline-flex items-center gap-1.5 text-xs font-semibold text-indigo-600 hover:text-indigo-700 transition-colors"
            >
              Посмотреть код на GitHub
              <ExternalLink class="w-3.5 h-3.5" />
            </a>
            <span v-else class="text-xs font-bold text-emerald-600 bg-emerald-50 px-2 py-0.5 rounded border border-emerald-100 uppercase tracking-wider">
              🚀 Действующий проект в работе
            </span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
