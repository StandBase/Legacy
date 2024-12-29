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
            margin-top: 50px;
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
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="glavv.html">Главная</a>
            <a href="shop.html">Магазин</a>
            <a href="forum.html">Форум</a>
        </nav>
        <div class="cabinet">
            <a href="#">Кабинет →</a>
        </div>
    </header>

    <div class="content">
        <h1 class="game-title">ARIZONA ROLE PLAY</h1>
        <p class="description">Многопользовательская онлайн игра с огромным открытым миром, в котором ты можешь стать кем захочешь!</p>
        <div class="button-container">
            <button class="button" onclick="location.href='shop.html'">Перейти в магазин</button>
        </div>
    </div>
</body>
</html>