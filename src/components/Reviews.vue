<template>
    <div class="container">
        <div class="flex-none gap-20 md:flex flex-row my-10 py-40 gap-10">
            <div class="basis-1/3"><!-- первый див сбоку -->
                <div class="flex justify-between items-center">
                    <h2 class="uppercase text-4xl whitespace-nowrap justify-self-center"><p class="text-flowergreen inline">Фото</p>хвасты</h2>
                    <a href="" class="text-flowergreen text-center text-lg underline decoration-dotted underline-offset-8 hover:text-flowergreendark transition">Больше фото</a>
                </div>
                <div class="mt-6 md:my-6 flex flex-wrap gap-3 md:gap-5"> <!-- див с фотками -->
                    <div><img src="/public/Rectangle 11.png" alt=""></div>
                    <div><img src="/public/Rectangle 11.1.png" alt=""></div>
                    <div><img src="/public/Rectangle 11.2.png" alt=""></div>
                    <div><img src="/public/Rectangle 11.3.png" alt=""></div>
                </div>

            </div>
            <div class="basis-2/3"> <!-- второй див -->
                <div class="flex mt-10 md:flex justify-between items-center">
                <h2 class="uppercase text-4xl whitespace-nowrap justify-self-center">Отзывы</h2>
                    <a href="" class="text-flowergreen text-lg underline decoration-dotted underline-offset-8 hover:text-flowergreendark transition">Смотреть все</a>
                </div>
                <div class="my-6">  <!-- сами отзывы -->
                    <div class="flex justify-between items-center">
                        <div><h3 class="text-lg text-flowergreen font-bold">Анатолий Петров</h3> <h4 class="text-sm">20.08.19 &nbsp; 22:32 &nbsp; &nbsp; г.Москва</h4></div> <div class="flex gap-1"><img src="/public/star.svg" alt="">  <img src="/public/staryellow.svg" alt=""> <img src="/public/staryellow.svg" alt=""> <img src="/public/staryellow.svg" alt=""> <img src="/public/staryellow.svg" alt=""></div>
                    </div>
                    <div class="my-3">
                        <h3 class="text-lg">Огромное спасибо флористам! Остались очень довольны оказанными услугами,мастера своего дела! Букетик даже неожиданно красивее чем на картинке</h3>

                    </div>
                </div>
                <div class="my-6">  <!-- сами отзывы -->
                    <div class="flex justify-between items-center">
                        <div><h3 class="text-lg text-flowergreen font-bold">Анатолий Петров</h3> <h4 class="text-sm">20.08.19 &nbsp; 22:32 &nbsp; &nbsp; г.Москва</h4></div> <div class="flex gap-1"><img src="/public/star.svg" alt="">  <img src="/public/staryellow.svg" alt=""> <img src="/public/staryellow.svg" alt=""> <img src="/public/staryellow.svg" alt=""> <img src="/public/staryellow.svg" alt=""></div>
                    </div>
                    <div class="my-3">
                        <h3 class="text-lg">Огромное спасибо флористам! Остались очень довольны оказанными услугами,мастера своего дела! Букетик даже неожиданно красивее чем на картинке</h3>

                    </div>
                </div>
                <div class="my-6">  <!-- сами отзывы -->
                    <div class="flex justify-between items-center">
                        <div><h3 class="text-lg text-flowergreen font-bold">Анатолий Петров</h3> <h4 class="text-sm">20.08.19 &nbsp; 22:32 &nbsp; &nbsp; г.Москва</h4></div> <div class="flex gap-1"><img src="/public/star.svg" alt="">  <img src="/public/staryellow.svg" alt=""> <img src="/public/staryellow.svg" alt=""> <img src="/public/staryellow.svg" alt=""> <img src="/public/staryellow.svg" alt=""></div>
                    </div>
                    <div class="my-3">
                        <h3 class="text-lg">Огромное спасибо флористам! Остались очень довольны оказанными услугами,мастера своего дела! Букетик даже неожиданно красивее чем на картинке</h3>

                    </div>
                </div>
            </div>
        </div>

    </div>
</template>

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
 img, video {
    max-width: max-content;
    height: auto; 
}
</style>