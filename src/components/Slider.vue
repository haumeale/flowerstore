<template>
    <div class="relative overflow-hidden">
        <div class="absolute w-full z-10">
      <Navigation />
    </div>
      <div
        class="w-full h-dvh flex transition-transform duration-1900"
        :style="`transform: translateX(-${currentSlide * 100}%)`"
      >
        <div v-for="(slide, index) in slides" :key="index" class="flex-shrink-0 w-full h-full">
          <div
            class="w-full h-full bg-cover bg-center flex items-center justify-center"
            :style="`background-image: url(${slide.image})`"
          >
          <div class="uppercase text-center text-midnight ">
            <h2 class="text-5xl font-bold py-5">
              <span class="text-flowergreen">{{ slide.titleHighlighted1 }}</span>  <!-- Первое выделенное слово -->
              <span class="">{{ slide.titleHighlighted2 }}</span>     <!-- Второе выделенное слово -->
            </h2>
            <p class="text-lg text-7xl">
              {{ slide.subtitlePart1 }} 
              <span class="text-8xl">{{ slide.subtitleHighlighted }}</span>  <!-- Выделенный подзаголовок -->
            </p>
            <button class="uppercase cursor-pointer text-xl mt-8 px-12 py-3 bg-flowergreen text-white rounded hover:bg-flowergreendark transition">
              Каталог
            </button> <!-- Кнопка добавлена здесь -->
          </div>
          </div>
        </div>
      </div>
  
      <div class="absolute bottom-4 left-1/2 transform -translate-x-1/2 flex space-x-2">
        <span
          v-for="(slide, index) in slides"
          :key="index"
          class="w-5 h-5 rounded-full cursor-pointer border-2 border-banerindicat"
          :class="{ 'bg-banerindicat': currentSlide === index,   
          'bg-transparent': currentSlide !== index }"
          @click="goToSlide(index)"
        ></span>
      </div>
    </div>
  </template>
  
  <script>
  import Navigation from './Navigation.vue';
  export default {
    components: {
    Navigation, // Добавляем компонент навигации в доступные компоненты
  },
    data() {
      return {
        currentSlide: 0,
        slides: [
          { image: '/public/baner1.png', 
          titleHighlighted1: 'Доставка ', 
          titleHighlighted2: 'цветов в город', 
        //   subtitlePart1: 'Это ', 
          subtitleHighlighted: 'Сочи', 
           },
          { image: '/public/baner2.png',
          titleHighlighted1: 'Слайд ', 
          titleHighlighted2: '1', 
        //   subtitlePart1: 'Это ', 
          subtitleHighlighted: 'подзаголовок', 
           },
          { image: '/public/baner3.png',
           titleHighlighted1: 'Слайд ', 
          titleHighlighted2: '1', 
        //   subtitlePart1: 'Это ', 
          subtitleHighlighted: 'подзаголовок', 
           },
        ],
        intervalId: null,
      };
    },
    methods: {
      nextSlide() {
        this.currentSlide = (this.currentSlide + 1) % this.slides.length;
      },
      goToSlide(index) {
        this.currentSlide = index;
      },
      startAutoSlide() {
        this.intervalId = setInterval(this.nextSlide, 6000); // Переключение слайдов каждые 3 секунды
      },
      stopAutoSlide() {
        clearInterval(this.intervalId);
      },
    },
    mounted() {
      this.startAutoSlide();
    },
    beforeUnmount() {
      this.stopAutoSlide();
    },
  };
  </script>
  
  <style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&family=Shantell+Sans:ital,wght@0,300..800;1,300..800&display=swap');

 h2 {
    font-family: "Shantell Sans", serif;
 }
 p {
    font-family: "Shantell Sans", serif;
 }

 button {
    font-family: "Shantell Sans", serif;
 }
</style>
  