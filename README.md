<!DOCTYPE html>
<html lang="cs">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Krimi</title>
    <style>
        /* Stylizace stránky s pohybujícím se zeleno-černým pozadím */
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #000000, #004d00, #000000);
            background-size: 200% 200%;
            animation: pozadiAnimace 15s ease-in-out infinite;
            color: #e6ffe6;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        /* Animace pro pohybující se pozadí */
        @keyframes pozadiAnimace {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* Navigační panel */
        .navbar {
            width: 100%;
            background-color: rgba(0, 0, 0, 0.7);
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
            padding: 10px 0;
            display: flex;
            justify-content: center;
        }

        .navbar a {
            text-decoration: none;
            color: #e6ffe6;
            margin: 0 20px;
            font-weight: bold;
            font-size: 1.2rem;
        }

        .navbar a:hover {
            color: #aaffaa;
        }

        /* Hlavní obsah */
        .main-content {
            text-align: center;
            padding: 20px;
            max-width: 1200px;
            width: 100%;
        }

        .section-title {
            font-size: 2rem;
            margin-top: 30px;
            color: #cc0000;
        }

        /* Styl karty pro krimi tématiku */
        .card {
            background-color: rgba(0, 51, 0, 0.8);
            padding: 20px;
            margin: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);
            color: #e6ffe6;
            display: inline-block;
            width: 250px;
            text-align: center;
            cursor: pointer;
            transition: transform 0.2s;
        }

        .card:hover {
            transform: scale(1.05); /* Zvětšení při najetí myší */
        }

        .card img {
            width: 100%;
            border-radius: 10px;
        }

        .card-title {
            font-size: 1.2rem;
            margin: 10px 0;
            color: #aaffaa;
        }

        /* Styl pro odkaz na stažení hry */
        .download-link {
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #cc0000;
            color: #ffffff;
            text-decoration: none;
            border-radius: 5px;
            font-size: 1.2rem;
            transition: background-color 0.3s;
        }

        .download-link:hover {
            background-color: #ff3333;
        }
    </style>
</head>
<body>
    <!-- Navigační panel -->
    <div class="navbar">
        <a href="#home">Domů</a>
        <a href="#games">Krimi Hry</a>
        <a href="#community">Komunita</a>
        <a href="#about">O nás</a>
    </div>

    <!-- Hlavní obsah -->
    <div class="main-content">
        <h1 class="section-title">Vítejte na Krimi</h1>
        <p>Objevte nejnovější krimi hry a připojte se ke komunitě milovníků detektivek a napětí.</p>

        <!-- Sekce Krimi Hry ve stylu karet -->
        <div id="games" class="section-title">Krimi Hry</div>
        <div class="card" onclick="window.location.href='https://example.com/game1';">
            <img src="game1.png" alt="Krimi Hra 1">
            <div class="card-title">Město Zločinu</div>
            <p>Staňte se detektivem a odhalte tajemství města plného záhad.</p>
        </div>
        <div class="card" onclick="window.location.href='https://example.com/game2';">
            <img src="game2.png" alt="Krimi Hra 2">
            <div class="card-title">Únik z vězení</div>
            <p>Pomožte nevinnému uprchnout ze spárů nespravedlnosti!</p>
        </div>
        <div class="card" onclick="window.location.href='https://example.com/game3';">
            <img src="game3.png" alt="Krimi Hra 3">
            <div class="card-title">Lovec Stínů</div>
            <p>Vyřešte zločiny a dopadněte tajemného pachatele.</p>
        </div>

        <!-- Odkaz na stažení hry -->
        <a href="http://tvá-domena.com/game.zip" class="download-link" download>Stáhnout Hru</a>
    </div>
</body>
</html>
