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
      <!-- Diamonds -->
      <div class="bg-gray-800 p-6 rounded-xl shadow">
        <h4 class="text-xl mb-2">Алмазы</h4>
        <p class="mb-2">Пополнение от 100 до 5000 алмазов. Быстрая доставка.</p>
        <button onclick="openModal('diamondsModal')" class="mt-4 bg-yellow-400 text-black px-4 py-2 rounded">Купить</button>
      </div>
      <!-- Vouchers -->
      <div class="bg-gray-800 p-6 rounded-xl shadow">
        <h4 class="text-xl mb-2">Ваучеры</h4>
        <p>Скидки на элитный пропуск, эксклюзивные предметы.</p>
      </div>
      <!-- Boosting -->
      <div class="bg-gray-800 p-6 rounded-xl shadow">
        <h4 class="text-xl mb-2">Прокачка</h4>
        <p>Помощь с ранговыми играми и прокачкой персонажей.</p>
      </div>
    </div>

    <!-- Categories -->
    <div class="mt-8 grid grid-cols-1 md:grid-cols-2 gap-6">
      <div class="bg-gray-700 p-4 rounded-xl">
        <h5 class="text-xl mb-2">🇷🇺 Для игроков из России</h5>
        <ul class="list-disc list-inside">
          <li>10.000 💎 — 6600 руб.</li>
          <li>20.000 💎 — 12.500 руб.</li>
          <li>30.000 💎 — 18.500 руб.</li>
          <li>50.000 💎 — 29.500 руб.</li>
        </ul>
      </div>
      <div class="bg-gray-700 p-4 rounded-xl">
        <h5 class="text-xl mb-2">🇰🇬 Для игроков из Кыргызстана</h5>
        <ul class="list-disc list-inside">
          <li>10.000 💎 — 6600 сом</li>
          <li>20.000 💎 — 12.500 сом</li>
          <li>30.000 💎 — 18.500 сом</li>
          <li>50.000 💎 — 29.500 сом</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- Modal -->
  <div id="diamondsModal" class="hidden fixed inset-0 bg-black bg-opacity-75 flex items-center justify-center z-50">
    <div class="bg-gray-800 p-6 rounded-xl w-full max-w-md">
      <h4 class="text-xl mb-4">Оформление заказа</h4>
      <label class="block mb-2">Выберите способ оплаты:</label>
      <select class="w-full mb-4 p-2 rounded bg-gray-700 text-white">
        <option>Крипта</option>
        <option>Банковская карта</option>
      </select>
      <label class="block mb-2">Вставьте номер карты/кошелька:</label>
      <input type="text" class="w-full mb-4 p-2 rounded bg-gray-700 text-white" placeholder="0000 0000 0000 0000" />
      <label class="block mb-2">ID аккаунта Free Fire:</label>
      <input type="text" class="w-full mb-4 p-2 rounded bg-gray-700 text-white" placeholder="123456789" />
      <div class="flex justify-end space-x-2">
        <button onclick="closeModal('diamondsModal')" class="px-4 py-2 rounded bg-gray-600">Отмена</button>
        <button class="px-4 py-2 rounded bg-yellow-400 text-black">Отправить</button>
      </div>
    </div>
  </div>

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
    <p>Свяжись с нами в Telegram: <a href="https://t.me/myxamet_ff" class="text-blue-400 underline">tologonov_m</a></p>
    <p>Email: <a href="mailto:freefire@mail.com" class="text-blue-400 underline">fasterff2021@gmail.com</a></p>
  </section>

  <!-- Footer -->
  <footer class="bg-gray-800 p-4 text-center">
    <p>&copy; 2025 Free Fire Магазин. Все права защищены.</p>
  </footer>

  <script>
    function openModal(id) {
      document.getElementById(id).classList.remove('hidden');
    }
    function closeModal(id) {
      document.getElementById(id).classList.add('hidden');
    }
  </script>
</body>
</html>
