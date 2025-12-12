# Sorteio-da-virada-25-26
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sorteio de Nomes</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #4a90e2, #9013fe);
            color: white;
            text-align: center;
            padding: 40px;
        }
        .container {
            background: rgba(255, 255, 255, 0.15);
            padding: 20px;
            border-radius: 12px;
            max-width: 450px;
            margin: auto;
            box-shadow: 0 4px 12px rgba(0,0,0,0.2);
        }
        button {
            background-color: #ffd700;
            color: #333;
            padding: 12px 25px;
            border: none;
            border-radius: 8px;
            font-size: 18px;
            cursor: pointer;
            margin-top: 20px;
            transition: 0.2s;
        }
        button:hover {
            background-color: #ffb300;
        }
        #resultado {
            margin-top: 25px;
            font-size: 26px;
            font-weight: bold;
            color: #fff;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Sorteio de Nomes</h1>
        <p>Clique no botão para sortear um vencedor:</p>

        <button onclick="sortear()">🎉 Sortear</button>

        <div id="resultado"></div>
    </div>

    <script>
        const nomes = [
            "Ana Cecília",
            "Ana Clara",
            "João Vitor",
            "Nilceu",
            "Bruno",
            "Nathalia",
            "Luciana",
            "Benedito",
            "Mavi",
            "Samuel",
            "Elaine",
            "Augusto",
            "Miguel",
            "Beatriz",
            "Zé do Santos"
        ];

        function sortear() {
            const indice = Math.floor(Math.random() * nomes.length);
            const vencedor = nomes[indice];
            document.getElementById("resultado").innerHTML =
                "🎉 <br> <strong>" + vencedor + "</strong>";
        }
    </script>

</body>
</html>
