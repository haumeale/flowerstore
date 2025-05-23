<script setup>
import Slider from './components/Slider.vue';
import Info from './components/Info.vue';
import Catalog from './components/Catalog.vue';
import FiveSteps from './components/FiveSteps.vue';
import Reviews from './components/Reviews.vue';
import Footer from './components/Footer.vue';
</script>

<template>
  <header class="text-white bg-midnight">
    <div class="container">
    <ul class="flex items-center justify-between gap-10 p-2">
      <li class="hidden xl:flex items-center gap-2"><img src="/public/adress.svg" alt=""><p class="text-flowergreen font-bold">г. Сочи,</p><p> ул. Роз, 15 А </p></li>
      <li class="flex items-center gap-2 font-bold"><img src="/public/phoneg.svg" alt="">+ 7 808 353 53 35  <p class="hidden xl:flex">+ 7 888 888 88 88</p> </li>
      <li class="flex items-center gap-2 font-bold"><img src="/public/cart (2).svg" alt=""> 150 000 руб.</li>
    </ul>
  </div>
  </header>
  <div>
    <Slider />
  </div>
  <div>
    <Info />
  </div>
  <div>
    <Catalog />
  </div>
  <div>
    <FiveSteps />
  </div>
  <div>
    <Reviews />
  </div>
  <div>
    <div class="container">
      <h3 class="text-lg">Букеты создаются максимально похожими на фотографию с сайта. Приведенные примеры букетов являются возможными вариантами составления цветочных композиций, так как они изготавливаются вручную флористами, и поэтому возможно незначительное отклонение по форме от фотографии на сайте. При этом возможна замена по количеству, ассортименту и составу цветов, в зависимости от сезонности, наличия цветов в том или ином регионе и других факторов на равноценные им по качеству и стоимости. Это позволит нам выполнить заказ без задержек. <br>
По России и странам СНГ доставка букета возможна в день оформления и оплаты заказа. По странам дальнего зарубежья доставка возможна через 2—3 рабочих дня после оплаты. <br>
Ближайшая дата и время доставки будут отображаться на странице оформления заказа с учетом выбранного города доставки. Мы рекомендуем оформлять и оплачивать заказы заранее, особенно в праздничный период. Более подробную информацию смотрите на страницеrr</h3>

    </div>
  </div>
  <div>
    <Footer />
  </div>
  
</template>

<style scoped>

</style>


<style>
.container{
  max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

body {
  color: #5B4A58;
}
</style>
