<script setup>
import Header from '@/components/Header.vue'
import CartList from '@/components/CardList.vue'
</script>

<template>
  <div class="bg-white w-4/5 m-auto rounded-2xl shadow-xl mt-14">
    <Header />
    <div class="p-10">
      <div class="flex justify-between items-center">
        <h1 class="text-3xl font-bold mb-8">Все кроссовки</h1>
        <div class="flex gap-5">

          <select class="py-2 px-3 border rounded-md outline-none">
            <option>По названию</option>
            <option>Сначала дешевые</option>
            <option>Сначала дорогие</option>
          </select>

          <div class="relative">
            <img class="absolute left-4 top-3" src="/search.svg" alt="Search" />
            <input
              class="border rounded-md py-2 pl-11 pr-4 outline-none transition focus:border-gray-400"
              placeholder="Поиск..."
            />
          </div>

        </div>
      </div>
      <CartList />
    </div>
  </div>
</template>
