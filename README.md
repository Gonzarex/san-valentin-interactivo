<!DOCTYPE htm>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Serás mi San Valentín?</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
            font-family: Arial, sans-serif;
            background-color: pink;
        }
        h1 {
            color: red;
        }
        .buttons {
            position: relative;
            margin-top: 20px;
        }
        button {
            font-size: 20px;
            padding: 10px;
            margin: 10px;
            cursor: pointer;
        }
        #no {
            position: absolute;
        }
    </style>
</head>
<body>
    <h1>¿Quieres ser mi San Valentín? ❤️</h1>
    <div class="buttons">
        <button id="yes">Sí 💖</button>
        <button id="no">No 💔</button>
    </div>

    <script>
        document.getElementById("yes").addEventListener("click", function() {
            alert("¡Yay! 💕 Nos vemos el 14 de febrero! 🎉");
        });

        document.getElementById("no").addEventListener("mouseover", function() {
            let x = Math.random() * window.innerWidth - 100;
            let y = Math.random() * window.innerHeight - 50;
            this.style.left = `${x}px`;
            this.style.top = `${y}px`;
        });
    </script>
</body>
</html>
