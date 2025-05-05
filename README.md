
<html lang="fi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kulmakonditoria</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #f5f5dce6; /* Vaalea beige tausta */
            color: #4b2e2e; /* Tumma ruskea teksti */
        }

        header {
            background-color: #cca31c; /* Kultainen väri */
            color: #4b2e2e; /* Tumma ruskea teksti */
            padding: 20px;
            text-align: center;
            position: relative;
        }

        .menu-button {
            position: absolute;
            top: 10px;
            left: 20px; /* Siirretty vasempaan yläkulmaan */
            width: 40px;
            height: 40px;
            background-color: #4b2e2e; /* Tumma ruskea */
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 18px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .menu-content {
            display: none; /* Piilotetaan oletuksena */
            position: absolute;
            top: 60px;
            left: 20px;
            background-color: #4d3737; /* Tumma ruskea */
            border: 1px solid #4b2e2e;
            border-radius: 5px;
            padding: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            z-index: 1000;
        }

        .menu-content a {
            display: block;
            color: #fff;
            text-decoration: none;
            padding: 5px 0;
        }

        .menu-content a:hover {
            background-color: #cca31c; /* Kultainen väri */
        }

        main {
            padding: 20px;
            text-align: center;
        }

        footer {
            background-color: #423131; /* Tumma ruskea */
            color: #ffffff;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>Kulmakonditoria</h1>
        <button class="menu-button" onclick="toggleMenu()">☰</button>
        <div class="menu-content" id="menuContent">
            <a href="menu.html">Menu</a>
            <a href="about.html">Tietoa meistä</a>
            <a href="contact.html">Yhteystiedot</a>
        </div>
    </header>
    <main>
        <section id="menu">
            <h2>Menu</h2>
            <p>Vuodesta 1996 asti leivottuja suuhunsulavia herkkuja</p>
            <p>Kulmanpuusti 4,30€</p>
            <p>Kahvi 1.50€</p>
            <p>Limut 2.5€</p>
            <p>Muut leivokset 4€</p>
            <p>Edellisen päivän tuotteet -50%</p>
            <p>Lämpimät ruoat seuraavalla sivulla!</p>
        </section>
        <section id="about">
            <h2>Tietoa meistä</h2>
            <p>Kulmakonditoria on perinteinen kahvila, joka tarjoaa laadukkaita tuotteita ja viihtyisän ilmapiirin.</p>
            <p>Meiltä löydät myös gluteenittomia ja vegaanisia vaihtoehtoja.</p>
            <img src="https://static.wixstatic.com/media/145316_30b59f53c13741189acc4c3561870cdd~mv2.jpg" alt="Kulmakonditoria" style="max-width:70%; height:auto;">
        </section>
        <section id="contact">
            <h2>Yhteystiedot</h2>
            <p>Osoite: Kauppakaari 8, 04200 Kerava</p>
            <p>Puhelin: 010 123 4567</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2025 Kulmakonditoria</p>
    </footer>
    <script>
        function toggleMenu() {
            const menu = document.getElementById("menuContent");
            if (menu.style.display === "block") {
                menu.style.display = "none"; // Piilota valikko
            } else {
                menu.style.display = "block"; // Näytä valikko
            }
        }
    </script>
</body>
</html>
