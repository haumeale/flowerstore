<template>
    <div class="mt-20">
        <div class="bg-brownfooter p-10">
            <div class="container">
                <div>
                    <ul class="flex justify-between text-lg text-white items-center">
                        <li>Каталог</li>
                        <li>Скидки</li>
                        <li>Отзывы</li>
                        <li>Контакты</li>
                        <li>Оферта</li>
                        <li class="flex gap-2 items-center text-white">Информация для клиента <img src="/public/Vector 2.svg" alt=""></li>
                    </ul>
                </div>
            </div>
        </div>
        <hr>
        <div class="bg-midnight">
            <div class="container">
                <div class="py-8 flex justify-between gap-10">
                    <ul class="text-white">
                        <h3 class="text-xl font-bold text-flowergreen my-4">Контактная информация</h3>
                        <li class="my-4 flex gap-3"><img src="/public/geo.svg" alt="">г. Владивосток, ул. <br> Пушкинская, 17</li>
                        <li class="my-4 flex gap-3"><img src="/public/phonef.svg" alt="">+ 7 888 888 88 88</li>
                        <li class="my-4 flex gap-3"><img src="/public/phonef.svg" alt="">+ 7 888 888 88 88</li>
                        <li class="my-4 flex gap-3"><img src="/public/clock1.svg" alt="">Режим работы: <br> 
                            Пн-Сб  с 8:00  до 22:00</li>
                    </ul>
                    <ul class="text-white">
                        <h3 class="text-xl font-bold text-flowergreen my-4">Для посетителей</h3>
                        <li class="my-4">Оформление заказа</li>
                        <li class="my-4">Вопросы и ответы</li>
                        <li class="my-4">Изменение или отмена заказа</li>
                        <li class="my-4">Способы доставки и оплаты</li>
                    </ul>
                    <div class="text-white">
                        <h3 class="text-xl font-bold text-flowergreen my-4">Возникли вопросы? Свяжитесь с нами</h3>
                        <div>
                            <Form />

                        </div>

                    </div>
                </div>
            </div>
        </div>
        <hr>
        <div class="bg-midnight p-8">
            <div class="container">
            <h3 class="text-white items-center opacity-55 text-center">© 2025 Цветочная лавка.</h3>
        </div>

        </div>
    </div>
</template>

<script>
import Form from './Form.vue';
export default {
    components: {
        Form, // Добавляем компонент навигации в доступные компоненты
  },
}

</script>

<style scoped>
hr {
    color: white;
}
</style>
