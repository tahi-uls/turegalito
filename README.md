<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Evelyn ❤️</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background: linear-gradient(to right, #ff758c, #ff7eb3);
            color: white;
            overflow: hidden;
        }
        .container {
            margin-top: 50px;
            animation: fadeIn 2s ease-in-out;
        }
        h1 {
            font-size: 2.5em;
            animation: fadeInDown 2s ease-in-out;
        }
        p {
            font-size: 1.2em;
            max-width: 600px;
            margin: 20px auto;
            animation: fadeInUp 2s ease-in-out;
        }
        .gallery img {
            width: 200px;
            height: auto;
            margin: 10px;
            border-radius: 10px;
            animation: zoomIn 1.5s ease-in-out;
        }
        .button {
            background-color: #ff4e50;
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1.2em;
            border-radius: 10px;
            cursor: pointer;
            transition: transform 0.3s ease;
            animation: fadeIn 3s ease-in-out;
        }
        .button:hover {
            transform: scale(1.1);
        }
        .music {
            position: fixed;
            top: 10px;
            right: 10px;
            background: rgba(255, 255, 255, 0.3);
            padding: 10px;
            border-radius: 50px;
            cursor: pointer;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        @keyframes fadeInDown {
            from { opacity: 0; transform: translateY(-50px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(50px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes zoomIn {
            from { transform: scale(0.8); opacity: 0; }
            to { transform: scale(1); opacity: 1; }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Hola Evelyn ❤️</h1>
        <p>Desde el primer día que te conocí hiciste sentir mi corazón muchas cosas y me hiciste sentir cosas únicas. 
            Créeme que desde ese día me he enamorado demasiado de ti y cada día te amo más. 
            Espero que aceptes ser mi San Valentín. 💖</p>
        
        <div class="gallery">
            <img src="foto1.jpg" alt="Foto 1">
            <img src="foto2.jpg" alt="Foto 2">
        </div>

        <button class="button" onclick="mostrarMensaje()">¿Aceptarás ser mi San Valentín?</button>

        <div class="music" onclick="toggleMusic()">🎵</div>

        <audio id="bg-music" loop>
            <source src="musica.mp3" type="audio/mp3">
            Tu navegador no soporta audio.
        </audio>
    </div>

    <script>
        function mostrarMensaje() {
            alert("¡Espero que sí! ❤️");
        }

        function toggleMusic() {
            var music = document.getElementById("bg-music");
            if (music.paused) {
                music.play();
            } else {
                music.pause();
            }
        }
    </script>
</body>
</html>
            
