<template>
    
        <div class="container">
          <div class="flex flex-row my-10 py-30 gap-10">
             <div class="basis-4/4"> <!--  главный див сбоку -->
                <ul class="hidden md:flex items-center text-slate-500 gap-10 ">
                    <li><p class="text-slate-600">Сортировать по:</p></li>
                    <ul class="flex items-center text-slate-500 gap-10 ">
                    <li>Новизне</li>
                    <li>Цена по возрастанию</li>
                    <li>Цена по убыванию</li>
                    <li>Популярности</li>
                  </ul>

                </ul>
                <ul class="flex items-center justify-between text-slate-500 gap-10 md:hidden">
                    <li>Сортирока/фильтр/поиск</li>
                    <li><img src="/public/Polygon.svg" alt=""></li>
                  

                </ul>


                <div class="my-8 w-auto h-auto">
                    <div class="flex flex-wrap justify-center gap-10">
                        <ProductCard />
                        <ProductCard />
                        <ProductCard />
                        <ProductCard />
                        <ProductCard />
                        <ProductCard />
                        <ProductCard />
                        <ProductCard />
                        <ProductCard />
                         <!-- Здесь будут карточки товаров -->
                    </div>
                   
                </div>
                <div class="justify-self-center"> <!--  див с показать ещё -->
            <a href="#" class="text-flowergreen underline decoration-dotted underline-offset-8 hover:text-flowergreendark transition">Показать ещё</a>

          </div>
            </div>
            <div class="hidden md:block basis-1/4"> <!--  главный див сбоку -->
                <form  action="" method="get">
                <input class="p-2 rounded-none outline-none" name="s" placeholder="Поиск" type="text">
                <button type="submit"><img src="/public/searchflower.svg" alt=""></button>
                </form>

                <div class="max-w-md mx-auto mt-10">
  <p class="text-slate-500 text-sm mb-3">Стоимость:</p>
  <div class="space-y-2">
    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:visible absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">до 2500 руб.</span>
    </label>

    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white  peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">2500 - 4000 руб.</span>
    </label>

    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">4000 - 6000 руб.</span>
    </label>

    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">от 6000 руб.</span>
    </label>
  </div>
</div>

<div class="max-w-md mx-auto mt-10">
  <p class="text-slate-500 text-sm mb-3">Букет с ...</p>
  <div class="space-y-2">
    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Розами</span>
    </label>

    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Тюльпанами</span>
    </label>

    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Гортензиями</span>
    </label>

    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Подсолнухами</span>
    </label>
    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Орхидеями</span>
    </label>
    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Ирисами</span>
    </label>
    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Лилиями</span>
    </label>
    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Герберами</span>
    </label>
  </div>
</div>

<div class="max-w-md mx-auto mt-10">
  <p class="text-slate-500 text-sm mb-3">Цветы упаковано</p>
  <div class="space-y-2">
    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:visible absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Букетом</span>
    </label>

    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white  peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">В корзине</span>
    </label>

    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">В коробке</span>
    </label>
  </div>
</div>

<div class="max-w-md mx-auto mt-10">
  <p class="text-slate-500 text-sm mb-3">Цветовая гамма</p>
  <div class="space-y-2">
    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Белая</span>
    </label>

    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Розовая</span>
    </label>

    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Красная</span>
    </label>

    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Желтая</span>
    </label>
    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Оранжевая</span>
    </label>
    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Бордовая</span>
    </label>
    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Синяя</span>
    </label>
    <label class="flex items-center cursor-pointer">
      <input type="checkbox" class="hidden peer" />
      <span class="h-5 w-5 select-none border-2 border-gray-300 rounded-md flex items-center justify-center mr-2 peer-checked:border-transparent peer-checked:bg-flowergreen relative">
        <!-- Галочка -->
        <svg class="w-3.5 h-3.5 text-white peer-checked:block absolute" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
      </span>
      <span class="peer-checked:font-bold">Фиолетовая</span>
    </label>
  </div>
</div>
 

            </div>
          </div>
          

        </div>
    
</template>

<script>
import ProductCard from './ProductCard.vue';
export default {
    components: {
    ProductCard, // Добавляем компонент навигации в доступные компоненты
  },
}

</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&family=Shantell+Sans:ital,wght@0,300..800;1,300..800&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Liter&display=swap');

 ul {
    font-family: "Liter", serif;
 }
 
</style>