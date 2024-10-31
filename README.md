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

        /* Text upozornění */
        .coming-soon {
            font-size: 1rem;
            color: #ff6666;
            font-style: italic;
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
        
        <!-- Aktivní odkaz na stažení pro Město Zločinu -->
        <a href="http://mestozlocinu.com/Assets/game1.zip" download>
            <div class="card">
                <img src="game1.png" alt="Krimi Hra 1">
                <div class="card-title">Město Zločinu</div>
                <p>Staňte se detektivem a odhalte tajemství města plného záhad.</p>
            </div>
        </a>
        
        <!-- Ostatní hry s upozorněním, že nejsou v provozu -->
        <div class="card">
            <img src="game2.png" alt="Krimi Hra 2">
            <div class="card-title">Únik z vězení</div>
            <p class="coming-soon">Tato hra není ještě v provozu.</p>
        </div>

        <div class="card">
            <img src="game3.png" alt="Krimi Hra 3">
            <div class="card-title">Lovec Stínů</div>
            <p class="coming-soon">Tato hra není ještě v provozu.</p>
        </div>
    </div>
</body>
</html>
