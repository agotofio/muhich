<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Магазин Free Fire</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Russo+One&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Russo One', sans-serif;
    }
  </style>
</head>
<body class="bg-gray-900 text-white">

  <!-- Модальное окно -->
  <div id="modal" class="fixed inset-0 bg-black bg-opacity-70 flex items-center justify-center z-50 hidden">
    <div class="bg-gray-800 p-6 rounded-xl w-full max-w-md space-y-4">
      <h2 class="text-xl text-yellow-400">Оформление заказа</h2>
      <p id="product-info" class="text-white"></p>
      <label class="block text-sm">ID вашего аккаунта:</label>
      <input type="text" class="w-full p-2 rounded bg-gray-700 text-white" placeholder="Введите ID">

      <label class="block text-sm mt-2">Способ оплаты:</label>
      <select class="w-full p-2 rounded bg-gray-700 text-white">
        <option>Криптовалюта</option>
        <option>Банковская карта</option>
      </select>

      <label class="block text-sm mt-2">Введите данные (если карта — номер):</label>
      <input type="text" class="w-full p-2 rounded bg-gray-700 text-white" placeholder="Пример: 5536••••••••••••">

      <div class="flex justify-end space-x-2 mt-4">
        <button onclick="closeModal()" class="bg-red-500 px-4 py-2 rounded hover:bg-red-600">Закрыть</button>
        <button class="bg-green-500 px-4 py-2 rounded hover:bg-green-600">Отправить</button>
      </div>
    </div>
  </div>

  <!-- Header -->
  <header class="bg-gray-800 p-4 shadow-md">
    <div class="container mx-auto flex justify-between items-center">
      <h1 class="text-2xl">Free Fire Магазин</h1>
      <nav class="space-x-4">
        <a href="#services" class="hover:text-yellow-400">Услуги</a>
        <a href="#reviews" class="hover:text-yellow-400">Отзывы</a>
        <a href="#contacts" class="hover:text-yellow-400">Контакты</a>
      </nav>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="text-center py-12 bg-cover bg-center" style="background-image: url('https://i.imgur.com/8T0oCOt.jpg');">
    <div class="bg-black bg-opacity-70 py-16 px-4">
      <h2 class="text-4xl mb-4">Прокачай свой аккаунт Free Fire!</h2>
      <p class="text-lg">Алмазы, ваучеры и многое другое по низким ценам</p>
    </div>
  </section>

  <!-- Services Section -->
  <section id="services" class="py-12 container mx-auto px-4">
    <h3 class="text-3xl mb-8 text-yellow-400">Наши услуги</h3>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
      <!-- Алмазы -->
      <div class="bg-gray-800 p-6 rounded-xl shadow">
        <h4 class="text-xl mb-2">Алмазы</h4>
        <p class="mb-4">Пополнение от 100 до 5000 алмазов. Быстрая доставка.</p>
        <div class="text-sm space-y-2">
          <p class="text-yellow-400">🇷🇺 Для игроков из России:</p>
          <ul class="list-disc list-inside">
            <li><button onclick="openModal('10.000 💎 — 6600 руб.')" class="hover:underline">10.000 💎 — 6600 руб.</button></li>
            <li><button onclick="openModal('20.000 💎 — 12.500 руб.')" class="hover:underline">20.000 💎 — 12.500 руб.</button></li>
            <li><button onclick="openModal('30.000 💎 — 18.500 руб.')" class="hover:underline">30.000 💎 — 18.500 руб.</button></li>
            <li><button onclick="openModal('50.000 💎 — 29.500 руб.')" class="hover:underline">50.000 💎 — 29.500 руб.</button></li>
          </ul>
          <p class="mt-4 text-yellow-400">🇰🇬 Для игроков из Кыргызстана:</p>
          <ul class="list-disc list-inside">
            <li><button onclick="openModal('10.000 💎 — 6600 сом')" class="hover:underline">10.000 💎 — 6600 сом</button></li>
            <li><button onclick="openModal('20.000 💎 — 12.500 сом')" class="hover:underline">20.000 💎 — 12.500 сом</button></li>
            <li><button onclick="openModal('30.000 💎 — 18.500 сом')" class="hover:underline">30.000 💎 — 18.500 сом</button></li>
            <li><button onclick="openModal('50.000 💎 — 29.500 сом')" class="hover:underline">50.000 💎 — 29.500 сом</button></li>
          </ul>
        </div>
      </div>

      <!-- Ваучеры -->
      <div class="bg-gray-800 p-6 rounded-xl shadow">
        <h4 class="text-xl mb-2">Ваучеры</h4>
        <p>Скидки на элитный пропуск, эксклюзивные предметы.</p>
      </div>

      <!-- Прокачка -->
      <div class="bg-gray-800 p-6 rounded-xl shadow">
        <h4 class="text-xl mb-2">Прокачка</h4>
        <p>Помощь с ранговыми играми и прокачкой персонажей.</p>
      </div>
    </div>
  </section>

  <!-- Reviews Section -->
  <section id="reviews" class="py-12 bg-gray-800 px-4">
    <div class="container mx-auto">
      <h3 class="text-3xl mb-8 text-yellow-400">Отзывы клиентов</h3>
      <div class="space-y-6">
        <div class="bg-gray-700 p-4 rounded-xl">
          <p>🔥 Очень быстро получил алмазы! Рекомендую!</p>
          <span class="text-sm text-gray-400">– Игрок123</span>
        </div>
        <div class="bg-gray-700 p-4 rounded-xl">
          <p>💎 Всё чётко, без обмана. Уже второй раз беру ваучеры.</p>
          <span class="text-sm text-gray-400">– FF_Pro</span>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contacts" class="py-12 container mx-auto px-4">
    <h3 class="text-3xl mb-8 text-yellow-400">Контакты</h3>
    <p>Свяжись с нами в Telegram: <a href="https://t.me/твойник" class="text-blue-400 underline">@твойник</a></p>
    <p>Email: <a href="mailto:freefire@mail.com" class="text-blue-400 underline">freefire@mail.com</a></p>
  </section>

  <!-- Footer -->
  <footer class="bg-gray-800 p-4 text-center">
    <p>&copy; 2025 Free Fire Магазин. Все права защищены.</p>
  </footer>

  <!-- JS -->
  <script>
    function openModal(product) {
      document.getElementById('modal').classList.remove('hidden');
      document.getElementById('product-info').textContent = 'Вы выбрали: ' + product;
    }

    function closeModal() {
      document.getElementById('modal').classList.add('hidden');
    }
  </script>
</body>
</html>
