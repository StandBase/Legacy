<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arizona Role Play</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(to bottom, #1a1a1a, #333333);
            color: white;
            text-align: center;
        }
        header {
            background: #1a1a1a;
            padding: 20px 0;
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
        }
        nav {
            display: flex;
            justify-content: center;
            gap: 20px;
        }
        nav a {
            color: white;
            text-decoration: none;
            font-size: 18px;
            padding: 10px 20px;
            border-radius: 5px;
            transition: background 0.3s;
        }
        nav a:hover {
            background: #444444;
        }
        .cabinet {
            position: absolute;
            top: 20px;
            right: 20px;
            background: #444444;
            padding: 10px 20px;
            border-radius: 5px;
        }
        .cabinet a {
            color: white;
            text-decoration: none;
            font-size: 18px;
        }
        .content {
            margin-top: 80px;
            padding: 20px;
        }
        .game-title {
            font-size: 36px;
            margin: 20px 0;
        }
        .description {
            font-size: 18px;
            line-height: 1.5;
            margin: 20px auto;
            max-width: 600px;
        }
        .button-container {
            margin: 30px 0;
        }
        .button {
            background: linear-gradient(to right, #ff007f, #8000ff);
            color: white;
            font-size: 18px;
            padding: 15px 30px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s;
        }
        .button:hover {
            background: linear-gradient(to right, #cc0066, #6600cc);
        }
        .container {
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
            background: #3E3E2D;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);
        }
        .section-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 20px;
        }
        .section-links a {
            color: #FFF8E1;
            text-decoration: none;
            padding: 10px 15px;
            background: #FFC107;
            border-radius: 5px;
            transition: background 0.3s, transform 0.2s;
        }
        .section-links a:hover {
            background: #FF9800;
            transform: scale(1.1);
        }
        .items {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        .item {
            background: #4E4E33;
            border-radius: 8px;
            text-align: center;
            padding: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
            transition: background 0.3s;
        }
        .item:hover {
            background: #FFEB3B;
            color: #2C2C1B;
        }
        .item img {
            width: 100%;
            height: auto;
            max-width: 300px;
            margin: 0 auto 10px;
            border-radius: 10px;
            object-fit: cover;
        }
        .item h3 {
            margin: 10px 0;
        }
        .price {
            font-weight: bold;
            color: #FF5722;
            margin: 10px 0;
        }
        .btn {
            background: #FFEB3B;
            color: #2C2C1B;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s, transform 0.2s;
        }
        .hidden {
            display: none;
        }
        .message {
            text-align: center;
            font-size: 18px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="#home">Главная</a>
            <a href="#shop">Магазин</a>
            <a href="#forum">Форум</a>
        </nav>
        <div class="cabinet">
            <a href="#">Кабинет →</a>
        </div>
    </header>

    <div id="home" class="content">
        <h1 class="game-title">ARIZONA ROLE PLAY</h1>
        <p class="description">Многопользовательская онлайн игра с огромным открытым миром, в котором ты можешь стать кем захочешь!</p>
        <div class="button-container">
            <button class="button">Начать игру</button>
        </div>
    </div>

    <div id="shop" class="container hidden">
        <div class="section-links">
            <a href="#" onclick="showSection('shop')">Магазин</a>
            <a href="#" onclick="showSection('misc')">Разное</a>
            <a href="#" onclick="showSection('vip')">VIP</a>
            <a href="#" onclick="showSection('skins')">Скины</a>
            <a href="#" onclick="showSection('cars')">Машины</a>
            <a href="#" onclick="showSection('accessories')">Аксессуары</a>
        </div>
        <div class="items">
            <div class="item">
                <img src="https://pc.rod-ins.com/resource/web/arizona/shop/cards/50049.jpg" alt="AZ Монета">
                <h3>AZ Монета</h3>
                <p>Донат валюта</p>
                <button class="btn" onclick="location.href='https://t.me'">Приобрести</button>
            </div>
            <div class="item">
                <img src="https://pc.rod-ins.com/resource/web/arizona/shop/cards/scm_pack2.jpg" alt="Набор Основателя">
                <h3>Набор Основателя</h3>
                <p>Случайный скин, рандомная машина, 15 000 000 виртов</p>
                <button class="btn" onclick="location.href='https://t.me'">100 рублей</button>
            </div>
            <div class="item">
                <img src="https://pc.rod-ins.com/resource/web/arizona/shop/cards/starting_capital_1.jpg" alt="Стартовый капитал №1">
                <h3>Стартовый капитал №1</h3>
                <p>10 500 000 виртов, 10 случайных ларцов</p>
                <button class="btn" onclick="location.href='https://t.me'">50 рублей</button>
            </div>
        </div>
    </div>

    <div id="forum" class="container hidden">
        <p class="message">Раздел в разработке. Пожалуйста, зайдите позже!</p>
    </div>

    <script>
        function showSection(sectionId) {
            document.querySelectorAll('.container').forEach(section => {
                section.classList.add('hidden');
            });
            document.getElementById(sectionId).classList.remove('hidden');
        }
    </script>
</body>
</html>
