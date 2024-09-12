<script setup>
import DrawerHead from '@/components/Drawer/DrawerHead.vue'
import CartItemList from '@/components/CartItemList.vue'
</script>

<template>
  <div class="fixed top-0 left-0 h-full w-full bg-black z-10 opacity-70" />
  <div class="bg-white w-96 h-full fixed right-0 top-0 z-20 p-8">
    <DrawerHead />
    <CartItemList />

    <div class="flex flex-col gap-5 my-7">
      <div class="flex gap-3">
        <span>Итого:</span>
        <div class="flex-1 border-b border-dashed" />
        <b>25000 тг</b>
      </div>
      <div class="flex gap-3">
        <span>Налог 5%:</span>
        <div class="flex-1 border-b border-dashed" />
        <b>3600 тг</b>
      </div>

      <button
        disabled=""
        class="bg-lime-500 w-full rounded-xl py-3 text-white transition cursor-pointer hover:bg-lime-600 active:bg-lime-700"
      >
        Оформить Заказ
      </button>
    </div>
  </div>
</template>
