<template>
    <div>
    <form id="contactForm" action="/submit" method="POST">
        <div class="flex gap-5">
            <div>
        <label for="name">Ваше имя</label><br>
        <input type="text" id="name" name="name" required><br>
    </div>
        <div>
        <label for="phone">Моб. номер</label><br>
        <input type="tel" id="phone" name="phone" required><br>
    </div>
        </div>
        
        <label for="message"></label>
        <textarea id="message" name="message" required></textarea><br>
        <div class="flex flex-row-reverse">
        <button type="submit">Отправить</button>
    </div>
    </form>
</div>
</template>

<style scoped>
        form {
            
            border-radius: 5px;
        }
        input, textarea {
            width: 100%;
            margin: 10px 0;
            padding: 10px;
            background-color: white;
            border-radius: 4px;
            color: black;
        }
        button {
            background-color: #5cb85c;
            color: white;
            border: none;
            padding: 10px;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #4cae4c;
        }
    </style>