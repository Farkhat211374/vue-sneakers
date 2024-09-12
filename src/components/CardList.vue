<script setup>
import Cart from '@/components/Card.vue'

const onClickAdd = () => {
  alert("Hello World!")
}

</script>
<template>
  <div class="grid grid-cols-4 gap-5">
    <Cart
      title="Мужские Кроссовки Nike Blazer Mid Suede"
      image-url="/sneakers/sneakers-1.jpg"
      :price="25990"
      :is-favorite="true"
      :is-added="true"
      :on-click-add="onClickAdd"
    />
  </div>
</template>
