<html lang="fi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kulmakonditoria</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            background-color: #f5f5dce6; /* Vaalea beige tausta */
            color: #4b2e2e; /* Tumma ruskea teksti */
            line-height: 1.6; /* Parantaa luettavuutta */
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
            left: 20px;
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

        main h2 {
            color: #cca31c; /* Kultainen väri */
            font-size: 24px;
            margin-bottom: 10px;
        }

        main p {
            margin: 10px 0;
        }

        main .highlight {
            font-weight: bold;
            color: #4b2e2e; /* Tumma ruskea */
        }

        footer {
            background-color: #423131; /* Tumma ruskea */
            color: #fff;
            text-align: center;
            padding: 10px;
            width: 100%;
            position: relative;
            bottom: 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Kulmakonditoria</h1>
        <p>Tervetuloa nauttimaan herkullisista leivonnaisista ja kahvista!</p>
        <button class="menu-button" onclick="toggleMenu()">☰</button>
        <div class="menu-content" id="menuContent">
            <a href="menu.html">Menu</a>
            <a href="about.html">Tietoa meistä</a>
            <a href="contact.html">Yhteystiedot</a>
        </div>
    </header>
    <main>
        <h2>Tietoa Kulmakonditoriasta</h2>
        <p><span class="highlight">Ravintola Kulma</span>, kotoisammin <span class="highlight">Kulmis</span>, on kotimainen perheyritys, joka on toiminut vuodesta 1996.</p>
        <p>Leivomme ja leikkaamme, pursotamme ja piperrämme, kokkaamme ja vatkaamme, loihdimme soossit, marinadit ja maukkaat lisukkeet kutkutellaksemme kaikkien herkkusuiden makunystyröitä.</p>
        <p>Kaiken kukkuraksi kehitämme koko ajan uusia makuja.</p>
        <h2>Toimipisteemme</h2>
        <p>Toimipisteitä meillä on:</p>
        <ul style="list-style-type: square; text-align: left; display: inline-block;">
            <li>Järvenpäässä</li>
            <li>Hyvinkäällä Kauppakeskus Willassa</li>
            <li>Vantaalla Kauppakeskus Tikkurissa ja Kauppakeskus Myyrmannissa</li>
            <li>Keravalla</li>
            <li>Riihimäellä</li>
        </ul>
    </main>

        <p>&copy; 2025 Kulmakonditoria</p>
   
    <script>
        function toggleMenu() {
            const menu = document.getElementById("menuContent");
            if (menu.style.display === "block") {
                menu.style.display = "none";
            } else {
                menu.style.display = "block";
            }
        }
    </script>
</body>
</html>
