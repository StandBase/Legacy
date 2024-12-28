<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AZ Coin Shop</title>
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background: #121212;
            color: #E0E0E0;
        }
        header {
            background: linear-gradient(90deg, #1f1f1f, #333333);
            padding: 20px;
            color: #E0E0E0;
            text-align: center;
            font-size: 24px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }
        nav {
            background: #1f1f1f;
            color: #E0E0E0;
            display: flex;
            justify-content: center;
            padding: 10px 0;
        }
        nav a {
            color: #E0E0E0;
            text-decoration: none;
            margin: 0 15px;
            padding: 10px 15px;
            border-radius: 5px;
            transition: background 0.3s, transform 0.2s;
        }
        nav a:hover {
            background: #333;
            transform: scale(1.05);
        }
        .container {
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
            background: #1e1e1e;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);
        }
        .item {
            display: flex;
            align-items: center;
            padding: 15px 10px;
            border-bottom: 1px solid #333;
        }
        .item:last-child {
            border-bottom: none;
        }
        .item img {
            width: 80px;
            height: 80px;
            border-radius: 10px;
            margin-right: 15px;
            object-fit: cover;
        }
        .item h3 {
            margin: 0;
            color: #FFFFFF;
        }
        .item p {
            margin: 5px 0 0;
            color: #BBBBBB;
        }
        .price {
            font-weight: bold;
            color: #FF5722;
        }
        .btn {
            background: linear-gradient(90deg, #ff4081, #7c4dff);
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s, transform 0.2s;
        }
        .btn:hover {
            transform: scale(1.05);
        }
        .hidden {
            display: none;
        }
        .message {
            text-align: center;
            font-size: 18px;
            color: #E0E0E0;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>AZ Coin Shop</h1>
    </header>

    <nav>
        <a href="#" onclick="showSection('main')">Главная</a>
        <a href="#" onclick="showSection('misc')">Разное</a>
        <a href="#" onclick="showSection('vip')">VIP</a>
        <a href="#" onclick="showSection('skins')">Скины</a>
        <a href="#" onclick="showSection('cars')">Машины</a>
        <a href="#" onclick="showSection('accessories')">Аксессуары</a>
    </nav>

    <div class="container" id="main">
        <div class="item">
            <img src="https://via.placeholder.com/80" alt="AZ Монета">
            <div>
                <h3>AZ Монета</h3>
                <p>Donat currency</p>
                <button class="btn" onclick="location.href='https://t.me'">Купить</button>
            </div>
        </div>

        <div class="item">
            <img src="https://via.placeholder.com/80" alt="Набор Основателя">
            <div>
                <h3>Набор Основателя</h3>
                <p>Случайный скин, рандомная машина и 15 000 000 виртов</p>
                <span class="price">100 рублей</span>
                <button class="btn" onclick="location.href='https://t.me'">Купить</button>
            </div>
        </div>

        <div class="item">
            <img src="https://via.placeholder.com/80" alt="Стартовый капитал №1">
            <div>
                <h3>Стартовый капитал №1</h3>
                <p>10 500 000 виртов, 10 случайных ларцов</p>
                <span class="price">50 рублей</span>
                <button class="btn" onclick="location.href='https://t.me'">Купить</button>
            </div>
        </div>
    </div>

    <div class="container hidden" id="misc">
        <p class="message">Раздел в разработке. Пожалуйста, зайдите позже!</p>
    </div>

    <div class="container hidden" id="vip">
        <p class="message">Раздел в разработке. Пожалуйста, зайдите позже!</p>
    </div>

    <div class="container hidden" id="skins">
        <p class="message">Раздел в разработке. Пожалуйста, зайдите позже!</p>
    </div>

    <div class="container hidden" id="cars">
        <p class="message">Раздел в разработке. Пожалуйста, зайдите позже!</p>
    </div>

    <div class="container hidden" id="accessories">
        <p class="message">Раздел в разработке. Пожалуйста, зайдите позже!</p>
    </div>

    <script>
        function showSection(sectionId) {
            // Hide all sections
            document.querySelectorAll('.container').forEach(section => {
                section.classList.add('hidden');
            });

            // Show the selected section
            document.getElementById(sectionId).classList.remove('hidden');
        }
    </script>
</body>
</html>
