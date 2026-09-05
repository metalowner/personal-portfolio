<script setup lang="ts">
import { Users2, MessageSquareIcon, Target } from 'lucide-vue-next'
</script>

<template>
  <section class="py-16 px-6 md:px-8 max-w-5xl mx-auto">
    <div class="text-center mb-12">
      <h2 class="text-3xl font-bold text-slate-900 tracking-tight">Как мы будем работать</h2>
      <p class="text-sm font-semibold text-slate-400 uppercase tracking-wider mt-2">Принципы, благодаря которым со мной комфортно</p>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      <!-- Вместе -->
      <div class="text-center flex flex-col items-center gap-3">
        <div class="p-3.5 bg-indigo-600 text-white rounded-2xl shadow-lg shadow-indigo-600/10">
          <Users2 class="w-6 h-6" />
        </div>
        <h3 class="font-bold text-slate-800 text-base mt-2">Делаем всё вместе</h3>
        <p class="text-xs md:text-sm text-slate-500 font-medium leading-relaxed">
          Я не пишу слепые ТЗ, чтобы пропасть на месяц. Мы регулярно созваниваемся, детально обсуждаем каждый шаг и разбираем вопросы вместе, чтобы продукт точно решал ваши задачи.
        </p>
      </div>

      <!-- Понятный язык -->
      <div class="text-center flex flex-col items-center gap-3">
        <div class="p-3.5 bg-indigo-600 text-white rounded-2xl shadow-lg shadow-indigo-600/10">
          <MessageSquareIcon class="w-6 h-6" />
        </div>
        <h3 class="font-bold text-slate-800 text-base mt-2">Простой язык</h3>
        <p class="text-xs md:text-sm text-slate-500 font-medium leading-relaxed">
          Никакого сложного программистского сленга, трехбуквенных аббревиатур или заумных терминов. Я говорю на человеческом языке бизнеса и объясняю технические детали на пальцах.
        </p>
      </div>

      <!-- Результат -->
      <div class="text-center flex flex-col items-center gap-3">
        <div class="p-3.5 bg-indigo-600 text-white rounded-2xl shadow-lg shadow-indigo-600/10">
          <Target class="w-6 h-6" />
        </div>
        <h3 class="font-bold text-slate-800 text-base mt-2">Фокус на конверсию</h3>
        <p class="text-xs md:text-sm text-slate-500 font-medium leading-relaxed">
          Мне важно не просто написать код сайта или приложения. Я оцениваю понятность UX-дизайна для вашей аудитории, читаемость текстов и реальную вероятность совершения покупки вашим клиентом.
        </p>
      </div>
    </div>
  </section>
</template>
