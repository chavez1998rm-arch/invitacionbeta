<meta name='viewport' content='width=device-width, initial-scale=1'/><meta name='viewport' content='width=device-width, initial-scale=1'/><!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Confirmación de Asistencia - Baby Shower de Gemelos</title>
    <style>
        /* Estilos generales */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }

        body {
            background-image: url('tony.gif'); /* URL directa de tu imagen de fondo */
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            color: #333;
            line-height: 1.6;
            padding: 20px;
        }

        .contenedor {
            max-width: 800px;
            margin: 0 auto;
            background-color: rgba(255, 255, 255, 0.85);
            border-radius: 15px;
            box-shadow: 0 0 15px rgba(0,0,0,0.1);
            padding: 30px;
            /* Animación de aparición gradual */
            animation: aparecer 1s ease-in-out;
        }

        /* Animación de aparición */
        @keyframes aparecer {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Título principal */
        .titulo-principal {
            font-size: 32px;
            color: #7a93ac;
            text-align: center;
            margin-bottom: 30px;
            font-weight: bold;
            /* Animación de movimiento suave */
            animation: mover 2s ease-in-out infinite alternate;
        }

        @keyframes mover {
            from {
                transform: translateY(0);
            }
            to {
                transform: translateY(-5px);
            }
        }

        /* Secciones de información */
        .seccion {
            margin-bottom: 25px;
            padding: 20px;
            background-color: rgba(253, 248, 245, 0.9);
            border-radius: 10px;
            /* Animación de aparición con retraso */
            animation: aparecer 1s ease-in-out 0.3s both;
        }

        .seccion h2 {
            font-size: 24px;
            color: #9a7b6f;
            margin-bottom: 15px;
            border-bottom: 2px solid #e0d0c8;
            padding-bottom: 8px;
        }

        .seccion p {
            font-size: 18px;
            margin-bottom: 10px;
        }

        /* Datos de la cuenta */
        .cuenta {
            background-color: rgba(240, 247, 244, 0.9);
        }

        .cuenta .numero-cuenta {
            font-size: 20px;
            font-weight: bold;
            color: #5a7d7c;
        }

        /* Botón de confirmación */
        .boton-confirmacion {
            text-align: center;
            margin-top: 30px;
            /* Animación de aparición con retraso */
            animation: aparecer 1s ease-in-out 0.6s both;
        }

        .boton {
            display: inline-block;
            padding: 15px 30px;
            background-color: #7a93ac;
            color: #ffffff;
            font-size: 20px;
            font-weight: bold;
            text-decoration: none;
            border-radius: 8px;
            transition: background-color 0.3s ease, transform 0.2s ease;
        }

        .boton:hover {
            background-color: #5a7b96;
            transform: scale(1.05);
        }

        /* Botón de música */
        .boton-musica {
            text-align: center;
            margin-top: 20px;
            /* Animación de aparición con retraso */
            animation: aparecer 1s ease-in-out 1.2s both;
        }

        .boton-musica button {
            padding: 10px 20px;
            background-color: #9a7b6f;
            color: #ffffff;
            font-size: 16px;
            font-weight: bold;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .boton-musica button:hover {
            background-color: #8a6b5f;
        }

        /* Mensaje final */
        .mensaje-final {
            text-align: center;
            margin-top: 20px;
            font-size: 18px;
            color: #9a7b6f;
            font-style: italic;
            /* Animación de aparición con retraso */
            animation: aparecer 1s ease-in-out 0.9s both;
        }

        /* Responsividad */
        @media (max-width: 600px) {
            .titulo-principal {
                font-size: 28px;
            }

            .seccion h2 {
                font-size: 22px;
            }

            .seccion p, .mensaje-final {
                font-size: 16px;
            }

            .boton {
                padding: 12px 25px;
                font-size: 18px;
            }

            .boton-musica button {
                padding: 8px 16px;
                font-size: 14px;
            }
        }
    </style>
</head>
<body>
    <div class="contenedor">
        <!-- Título principal -->
        <h1 class="titulo-principal">Confirmación de Asistencia</h1>

        <!-- Sección de ubicación -->
        <div class="seccion">
            <h2>Ubicación</h2>
            <p>Dirección: 10 calle 5-51 entre 5ta y 6ta ave. barrio el rosario Amatitlán</p>
        </div>

        <!-- Sección de fecha y hora -->
        <div class="seccion">
            <h2>Fecha y Hora</h2>
            <p>Fecha: 14 de Marzo 2026</p>
            <p>Hora: 14:00 hrs</p>
        </div>

        <!-- Sección de regalos -->
        <div class="seccion cuenta">
            <h2>Regalos</h2>
            <p>Si es de tu agrado obsequiarnos un presente, que sea para gemelos unisex. Para tu comodidad, ponemos a tu disposición el siguiente número de cuenta:</p>
            <p class="numero-cuenta">No. 3164072404</p>
            <p>Monetaria Banrural</p>
        </div>

        <!-- Botón de confirmación con enlace de WhatsApp -->
        <div class="boton-confirmacion">
            <a href="https://wa.link/ee2ko7" class="boton" target="_blank">Confirmar Asistencia</a>
        </div>

        <!-- Botón de música -->
        <div class="boton-musica">
            <button id="botonMusica" onclick="toggleMusica()">Reproducir Música</button>
        </div>

        <!-- Mensaje final -->
        <p class="mensaje-final">No olvides confirmar tu asistencia a este día tan especial</p>
    </div>

    <!-- Melodía de fondo -->
    <audio id="audio" loop>
        <source src="Tony Tony Chopper.mp3" type='audio/mpeg'>
        <type="audio/mpeg"> 
    

    <script>
        // Función para reproducir o pausar la música
        function toggleMusica() {
            const audio = document.getElementById('audio');
            const boton = document.getElementById('botonMusica');
            
            if (audio.paused) {
                audio.play();
                boton.textContent = 'Pausar Música';
            } else {
                audio.pause();
                boton.textContent = 'Reproducir Música';
            }
        }

        // Si quieres que la música inicie automáticamente, descomenta la línea siguiente:
        // window.onload = function() { toggleMusica(); };
    </script>
</body>
</html>
